参考 [Git - Book](https://git-scm.com/book/zh/v2)

## Hooks

Hooks 可以实现在部分动作后，触发额外的脚本。初始化 git 项目时，会在 `.git/Hooks`  目录中生成一些 sample 文件。

举个例子，这个站点的 md 源文件放在 `writing/notes` 目录中，但是站点对应的项目是 [xiang578/gru](https://github.com/xiang578/gru)。每一次更新笔记后，需要手动将文件从 `writing/notes` 复制到 `gru/docs`，然后再 push 到 github 中编译部署。