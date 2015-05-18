# pythonMultiProcessAndThreadExamples
这里是一些和python多线程多进程相关的示例代码

For 树莓派兴趣小组分享

Author: 陈征cuc 中国传媒大学 计算机与网络中心 

##github:  源代码下载地址
  https://github.com/chenzheng128/pythonMultiProcessAndThreadExamples

##Python 多进程处理 LXF01 
Source: 廖雪峰: Python的小白教程  http://www.liaoxuefeng.com/wiki/001374738125095c955c1e6d8bb493182103fac9270762a000

##Python 多线程处理 LXF02


##Python Socket网络编程
###echo server 
  处理网络echo
###file server py
  client提供(文件名\文件信息), 上传文件至server


注意:

1. 线程共享数据, 需要上锁保护; 进程不共享, 需要通过Queue等方式共享

2. Windows 无法fork复制进程的状态以及文件句柄, 而是利用pickle来打包传递数据对象.因此在windows下的多进程网络编程常常会报错误. 因此子进程不能拿到真正的文件句柄
