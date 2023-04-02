# Vscode+Github

## 资料

https://code.visualstudio.com/docs/sourcecontrol/overview

推送安装插件：

GitHub Pull Requests and Issues

Git开启

一般来说，创建了仓库之后，在github网页打开的时候会有对应的添加本地的方式，打开Git Bash按照命令一步一步输入就能添加完成，之后就能正常推送了，需要注意走不走代理的问题，如果出现端口的问题可以用：

```
git config --global http.proxy  # 查看推送有没有走代理
git config --global --unset http.proxy # 取消代理之后可以正常的推送
```

然后继续输入报错的命令就行了。

查看状态:

```
git config --list
```

设置代理：

```
set http_proxy=http://127.0.0.1:1080
set https_proxy=http://127.0.0.1:1080
```

全局：

```text
git config --global http.proxy http://127.0.0.1:10808
git config --global https.proxy http://127.0.0.1:10808
```

取消全局：

```
git config --global --unset http.proxy
git config --global --unset https.proxy
```

socket5

```
git config --global http.https://github.com.proxy socks5://127.0.0.1:10808
git config --global https.https://github.com.proxy socks5://127.0.0.1:10808
```

## 已经存在仓库

直接打开想把文件夹存放的位置，然后git bash：

```bash
git clone 仓库url
```

直接clone下来就能正常推送了，需要记得填写更改消息就能避免面的情况.
