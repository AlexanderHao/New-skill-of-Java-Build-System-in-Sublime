# New-skill-of-Java-Build-System-in-Sublime
今天Google如何在ST中编译运行Java的时候，无意中发现了一个更好的方法。

其实，在ST中是可以编译Java的，但是运行不了，因为没有配置运行命令。那么一般的配置方法都是如下的：

http://www.oschina.net/translate/compile-and-run-java-programs-in-sublime-text-2

http://my.oschina.net/tashi/blog/187547

上面的方法，需要写runJava.bat放到jdk/bin下面，感觉侵入拖沓。

于是，Google了一下国外的技术文章，发现了一个youtube讲解视频 How to setup Java in Sublime Text 3 - (OS - Windows)：

https://www.youtube.com/watch?v=5yEq4_ap_XA

用很简单的方法，就可以编译运行Java。不能FQ的同学，在这里简单说下配置方法。在ST中点击Preferences->Browser Packages，在打开的文件夹下，会有个User文件夹，打开，在其中新建MyJavaC.sublime-build，用ST打开，编辑内容如下：
除了替换 "path": "C:\\Program Files\\Java\\jdk1.7.0_13\\bin\\", 为你自己的JDK Path以外，其它都无需改动。保存后，在包含Main入口方法的Java文件下，ctrl+shift+b，选择刚才自定义的MyJavaC，编译运行即可。

 
