# MkDocs

启动服务

```shell
mkdocs serve
```

## 自定义域名不生效

[将包含自定义域名 CNAME 文件复制一份到 docs/](https://mkdocs.zimoapps.com/user-guide/deploying-your-docs/#_2)

## Google Analytics 不生效

现象：Safari 生效，Edge/Chome 不生效。

打开浏览器的 `开发者工具-控制台` 出现如下错误：

```
Tracking Prevention blocked a Script resource from loading https://www.google-analytics.com/analytics.js.
GET https://www.google-analytics.com/analytics.js net::ERR_BLOCKED_BY_CLIENT
```

[Tag Assistant Legacy (by Google) - Chrome Web Store](https://chrome.google.com/webstore/detail/tag-assistant-legacy-by-g/kejbdjndbnbjgmefkgdddjlbokphdefk?hl=en)：Google 官方提供浏览器插件，帮助检查页面是否正确安装 GA。

## 参考

- [Getting Started - GiantPandaCV](http://giantpandacv.com/)


