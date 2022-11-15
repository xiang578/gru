```dataviewjs
let ftMd = dv.pages("").file.sort(t => t.cday)[0]
let total = parseInt([new Date() - ftMd.ctime] / (60*60*24*1000))
dv.paragraph(
	"距今已使用 "+total+" 天"
)
```


```dataviewjs
let nofold = '!"templates"'
let allFile = dv.pages(nofold).file
let totalMd = "共创建 "+
	allFile.length+" 篇文档"
let totalTag = allFile.etags.distinct().length+" 个标签"
let totalTask = allFile.tasks.length+" 个待办 <br><br>"
dv.paragraph(
	totalMd+"、"+totalTag+"、"+totalTask
)
```

## 进行中

```dataview
list
from #inbox 
sort file.ctime desc
```

```dataviewjs
dv.paragraph(
  dv.pages("").file.etags.distinct()
  .sort(t => dv.pages(t).length , 'desc')
  .map(
  	t => {
		return `[${t}](${t})`+"("+dv.pages(t).length+")"
	}
  ).array().join(" ")
)
```

## 最近编辑
```dataview
table WITHOUT ID file.link AS "标题",file.mtime as "时间"
from !"archive"
sort file.mtime desc
limit 5
```

## 最近创建

```dataview
table WITHOUT ID file.link AS "标题",file.ctime as "时间"
from !"archive"
sort file.ctime desc
limit 5
```

## 归档

```dataview
table WITHOUT ID rows.file[0].day.year+"年"+rows.file[0].day.month+"月" as 月份,length(rows)+"篇" as 数量
where !contains(file.folder, "templates")
group by file.day.month
```