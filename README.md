# new-ysoserial.net-exe
compile the latest version. 

在使用过程中，发现由testnull大佬提交的ClaimsPrincipal链没有被增加到最新版本的release中，而且我自己在编译过程中遇到了一些问题，花了一些时间才解决，希望我自己编译的版本可以有所帮助。

问题为：C# 尝试还原程序包时出错:找不到“XXXXX”版本的程序包“XXXXXX”
解决方案：首先将项目的.NET版本设置为4.6.1，其他版本可能也可以，但是我这里是这样设置的。然后将工具-》NuGet包管理器-》程序包管理设置中的程序源增加一项：
![image](https://user-images.githubusercontent.com/22125281/168267122-56c0fdf3-d1e0-4123-a1b1-8961bf8e01ac.png)
再到NuGet管理包处将所有没有找到的包都进行还原或者安装。之后就可以正常生成ysoserial.net的exe了。
