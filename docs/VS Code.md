
## Code Server

[cdr/code-server: VS Code in the browser](https://github.com/cdr/code-server)：服务器版本 VS Code。由于公司内部服务器需要在堡垒机上跳转登陆，无法直接使用 VS Code Remote 。服务器安装后，可以在本地网页上使用 VS Code。

## 问题

### 解决 Vim mode 和输入法的冲突，自动切换输入法状态

- 参考 [VSCodeVim/Vim input-method](https://github.com/VSCodeVim/Vim#input-method) 实现」在 vim insert 时，输入法是中文，切换到 normal 同时将输入法切换成英文」。
- 上面的插件需要搭配 [daipeihust/im-select: Switch your input method through terminal 📟](https://github.com/daipeihust/im-select#installation) 使用
	- 直接下载需要的 bin `curl -L -o /usr/local/bin/im-select https://github.com/daipeihust/im-select/raw/master/im-select-mac/out/im-select`
	- 我使用的英文输入法是 `com.apple.keylayout.ABC`，中文输入法是 `im.rime.inputmethod.Squirrel.Rime`
	- VS code setting 中找到 autoSwitchInputMethod，参考下面配置：
		- ![autoSwitchInputMethod](https://media.xiang578.com/autoSwitchInputMethod.png)	
