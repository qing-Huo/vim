# vim
vim配置相关


原文链接:https://blog.csdn.net/Liukairui/article/details/107392243



## win10下,给git配置代理
	git config --global https.proxy http://127.0.0.1:1080

	git config --global https.proxy https://127.0.0.1:1080
	
	查看代理
	
	git config --global --unset http.proxy
	
	git config --global --unset https.proxy





## 装插件之前必要的准备

​	需要安装 python 并加入环境变量(并且要置顶)

​	在gvim中输入 :version 可以查看gvim对python的支持, python 安装符合 gvim 的版本即可

​	在 gvim 中输入命令 :echo has("python3"),这里一定要是字符串的python3

​	如果输出 1, 说明成功

​	之后在输入 :python3 print("123“）,看到字符串输出即代表成功





## 全语言代码自动补全  YouCompleteMe

​	按照原作内容:先下载插件

​							之后写入配置

​							下载安装`clang`与`cmake`并加入环境变量

​							安装VS (具体版本以插件地址提供为准),这里我用的是2019,只选择C++生成工具

							安装后打开插件安装地址，按住shift，右键，点击打开powershell

​							输入命令`Python install.py --all` 这个过程很慢,毕竟是全语言补全,也可以只装对应的语言,比如我用js,那么把上面的 --all 换成 --js-completer即可
								
​							