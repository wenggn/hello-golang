# 这是一个学习项目

> 通过学习《如何使用 Go 编程》，写的第一个 Go 程序，详情见：[如何使用Go编程](http://docscn.studygolang.com/doc/code.html)
>
> 注：这里将 `stringutil` 库放在了 `hello-golang` 中，仅仅是为了统一源码管理。

## Go for Visual Studio Code

在安装完go扩展之后，有一些依赖包还需要进一步安装，一般在使用vscode打开.go文件时触发安装，往往会安装失败，golang.org 在国内由于一些众所周知的原因无法直接访问。

下面这些内容是网上摘录的，已验证。（总的来说就是不能访问的内容github.com上也有，手动下载然后安装即可）

### 解决github.com访问慢的问题（可选）
>
> 编辑`C:\Windows\System32\drivers\etc\hosts`文件，添加
>
>```txt
>192.30.253.113      github.com
>151.101.77.194      github.global.ssl.fastly.net
>```
>
>最后刷新缓存 `ipconfig /flushdns`

### 手动下载安装依赖包
>
>```bash
>cd %GOPATH%\src\golang.org\x
>git clone https://github.com/golang/tools.git tools
>git clone https://github.com/golang/lint
>```
>
>重新打开vscode，然后继续安装。
