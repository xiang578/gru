[[Niklas Luhmann]]


- 原则
    - 原子化：每一篇笔记尽可能围绕一个主题
    - 笔记之间相互链接形成一个网状：
        - ![](https://media.xiang578.com//link-notes.png)
    - 在 [[wiki link]] 基础上更进一步 "link your notes and explain why you arr linking notes"。不一定都能被关键词给链接在一起。如果简单使用关键词连接，那么写一个脚本就能把所有的内容链接在一起。
    - 利用 tags 取代分类：[[Bear]] 中就支持
        - ![](https://media.xiang578.com//tag.png)
    - 用自己的语言总结替代全文收集，将文章剪藏移到其他软件中。
    - 定期回顾笔记
- 集中收集资料和想法，创造价值
- 使用
    - 每日笔记记录阅读的文章，通过引用放到其他页面下集中。

    - 每日笔记记录阅读的文章，通过引用放到其他页面下集中。


- 是否公开
    - 逛其他人的个人wiki可能是一件有趣的事情，特别是能顺着笔记一篇篇阅读下去。

- [[blog Zettelkasten]] 

主流知识管理软件设计偏向于树型结构，从软件开发的角度来说，便于进行存储和层次化遍历。知识卡片通过链接连接在一起达到网状的效果。

常规笔记方法，比如在一本书上做标记和写心得，这样的笔记很难有很大的意义。

他开始思考一个想法如何与不同情境相联系、如何应用于不同情境。仅仅在一个地方存放笔记除了产生一堆笔记，并不能产生其他任何东西。

[ ] 是不是需要两个卡片盒？文献卡片盒以及想法卡片盒

ID, tags, link

structure notes: 定期对笔记进行整理和汇总

1. Notes are atomic: single bit of information.
2. Each Note Has a Home: 
3. Each Note Has a Name: unique ID
4. Notes Link to other Notes
5. Cross Reference Keywords

ID 是为了相互链接，但是我认为这个是低效的，ID 太多，你很难看到一个 ID 可以想到他是什么内容，最好的方法是看 ID 对应的那个标题。
内容要少，像现在这篇笔记就是错误的示范……
人工手动链接笔记。

> 20200213 在 [Some Thoughts on How to Keep a Zettelkasten – trms blog](https://trms.me/some-thoughts-on-how-to-keep-a-zettelkasten/) 中发现一点：对于部分不支持 wiki link 的软件中，双击快速选择数字 ID 做为关键字，然后可以配合软件中的快速跳转打开这个文档。但是还不如支持 wiki link 的软件方便。


笔记数量太多还能有效的管理吗？

现实中，NL 使用不同的盒子管理笔记，所以我们也可以使用文件夹去归档笔记。但是从本质上来说，还是需要减少用文件夹来聚合内容，系统又很大的奔溃风险。通过 tag + link 来聚合内容。
现实中相关的卡片可以放在一起保存，对应到软件中，可以使用文件夹来区分，但是需要减少时间在设计文件夹系统上。
zk 用来记录有长时间价值的内容，由自己产生。

[The Archive](the-archive.md) 中可以保存搜索，实现快速查找某一类的文件。

觉得软件配色很漂亮，不代表学到什么，记住什么。

临时卡片、文献卡片、永久卡片


文献卡片：对任何读过的内容做笔记。
永久笔记：想想笔记和自己当前研究、思考和兴趣的关联。

nl 提倡卡片尽量只包含一个观点，卡片上能写的内容受限于卡片的大小，如果用软件来实现，需要避免超长的文本。



## 原则

1. 原子性：一篇笔记尽可能只包含一个观点以及尽可能的短。
2. 相互链接：不同笔记之间需要人工进行链接。
3. 简单的注释，在不同笔记之间进行链接时，做一些简单的说明。
4. 用自己的话，不用简单复制和粘贴，记录自己的语言
5. 添加参考资料，说明从哪里获得的灵感
6. 利用 zettlkasten 的原则迭代这套方法
7. 不要对笔记进行分类，使用 structure note 替代，自己制作归档页面
8. 大纲笔记，归档想法
9. 不要删除笔记，用新笔记说明为什么要删除旧笔记，通过这种方法见证自己的成长



## 实践

从需求出发选择软件：

1. markdown + latex 公式
2. 插入图片
3. 文档链接，点击后可以跳转到目标文档，反向链接（告诉你该文档被那些文档引用）
4. 搜索（关键词（标签），链接）
5. 文档之间的引用关系
6. 不同设备之间同步，文档备份
7. 历史信息（git）

最后回到 Mweb 的怀抱

[文档库模式下,md文件的互相跳转 · Issue #169 · oulvhai/MWeb-issues](https://github.com/oulvhai/MWeb-issues/issues/169)

改进

- 放弃使用日期之类的 UID，利用关键词命名文档。

[Knowledge Management with Zettelkasten and iA Writer – trms blog](https://trms.me/knowledge-management-with-zettelkasten-and-ia-writer/)

[[Zettelkasten 编码]]