# 背景
本文档所有操作均在win11下完成 
# 学习前的准备
- 一颗赤诚的心
- 熟练使用Google
- 梯子(VPN)----计算机学生必备

# 学习使用Github
(一般需要使用梯子,校园网可以连,但是不稳定)  

<https://zhuanlan.zhihu.com/p/369486197>  

ssh配置  

<https://blog.csdn.net/weixin_42310154/article/details/118340458>

# 安装WSL(类似双系统)
___本次培训接下来配置环境可以选择在linux中配置,也可以在win11环境下运行,一般推荐在linux环境中运行ai项目___  
___经测试本次实验可以在win11环境下运行___  

<https://bilibili.com/read/cv16825907>
<https://juejin.cn/post/7173582392064475150>    

>
>注意问题 如果存在应用商店网络问题，可以尝试使用Host修改工具
>
>(www.dogfight360.com/blog/475/)
>
>每个人的电脑有独属于自己的问题 最好查询google


# 基础知识

## 学习使用Github
(一般需要使用梯子,校园网可以连,但是不稳定)  

<https://zhuanlan.zhihu.com/p/369486197>  

ssh配置  

<https://blog.csdn.net/weixin_42310154/article/details/118340458>

## 安装WSL(类似双系统)
___本次培训接下来配置环境可以选择在linux中配置,也可以在win11环境下运行,一般推荐在linux环境中运行ai项目___  
___经测试本次实验可以在win11环境下运行___  

<https://bilibili.com/read/cv16825907>
<https://juejin.cn/post/7173582392064475150>    

>
>注意问题 如果存在应用商店网络问题，可以尝试使用Host修改工具
>
>(www.dogfight360.com/blog/475/)
>
>每个人的电脑有独属于自己的问题 最好查询google

## 了解windows 的cmd powershell之间的区别  

<https://hackmd.io/@__HTwCNgSRaw2rSxRS-R-g/Byz832gRj>
上述的操作都可以用几行命令完成,这就是计算机的魅力  

win+x 呼唤出windows命令工具 在按一次I呼唤出终端  

或者使用   

win+r 输入cmd 呼唤出cmd  

![](img\1.png)
![](img\2.png)


# 以下推荐两种配置方法
- 传统配置方法
- scoop(windows下的包管理工具)
## 安装miniconda()  

请阅读下列教程   

阅读完再开始操作  

<https://blog.csdn.net/Loveful/article/details/132412037>  

[https://blog.csdn.net/qq_40597075/article/details/122560335](https://blog.csdn.net/qq_40597075/article/details/122560335)  

>注 安装时推荐选择`just me`以及`自动配置环境变量`的选项
## 下载vscode  

<https://code.visualstudio.com/download>  

### 配置python和jupyter  

<http://www.kaixinit.com/info/python/9186.html>   

(忽略其中的anaconda部分,其实anaconda和miniconda很像,但是体积太大,电脑在512g内存及以下的慎装)  

<https://cangmang.xyz/articles/1642849032438>
## scoop 拥抱终端 未曾设想的道路   

先阅读下列教程  

<https://p3terx.com/archives/scoop-the-best-windows-package-manager.html>  

<https://zhuanlan.zhihu.com/p/128955118?utm_id=0>

设置配置路径(设置完之后你的文件都会下载到这里)
```
#此时需要管理员权限
$env:SCOOP='D:\Scoop'
[Environment]::SetEnvironmentVariable('SCOOP', $env:SCOOP, 'User')
$env:SCOOP_GLOBAL='D:\Scoop_Global'
[Environment]::SetEnvironmentVariable('SCOOP_GLOBAL', $env:SCOOP_GLOBAL, 'Machine')
```
输入下列命令安装scoop(以下均在在powershell中输入)
```
#此时不可以是管理员权限
Set-ExecutionPolicy RemoteSigned -scope CurrentUser
irm get.scoop.sh | iex
```

安装wsl
```
scoop install wsl
```
安装miniconda
```
scoop install miniconda
```
安装Visual Studio Code (VSCode)
```
scoop install vscode
```

