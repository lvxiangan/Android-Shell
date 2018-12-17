# Android-Shell
Android实现对APK加壳demo，通过cmake实现JNI


AndroidShell
其中两个android源程序对应的android studio版，使用了cmake 方式实现JNI

Step1：打包demo工程：demo.apk
Step2（先设置解壳/密）：打包解壳工程：shell.apk，解压获取：shell.dex
Step3（开始加壳/密）：运行java工程，合并shell.dex和demo.apk，得到：classes.dex
step4（修正签名、运行）：把class.dex放进shell.apk，重新签名得到：shell_demo.apk
shell_demo.apk就是我们想得到的加壳app！


相关博客：http://blog.csdn.net/yongaini10/article/details/52275788

参考： http://blog.csdn.net/androidsecurity/article/details/8678399

  https://github.com/longtaoge/AndroidShell
