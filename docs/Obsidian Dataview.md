#pubilc 

标签 `= this.file.tags`

所有标签列表
```dataviewjs
// 生成所有的标签且形成列表
dv.list(dv.pages("").file.tags.distinct())
```

## 示例

````text
在此文件中放置两个标签 #OK1  #OK2 用于对比测试.

// 此文件内标签 

`= this.file.tags`

// 所有标签列表
```dataviewjs
// 生成所有的标签且形成列表
dv.list(dv.pages("").file.tags.distinct())
```

// 按时间进行过滤
```dataview
table file.ctime from #D3 where file.ctime > date(2021-03-28) - dur(3 days)
```

// 按时间和文件名过滤
```dataview
table file.ctime from #D3 where file.ctime > date(2021-03-28) - dur(3 days)
and contains(file.name, "20")
```

// 查询标签下内容并返回列表
```dataview
list from #D3 where file.ctime > date(2021-03-28) - dur(3 days)
```

// 按块搜索并返回
在Obsidian搜索栏使用行语法搜索line:()
````