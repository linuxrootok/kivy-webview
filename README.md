# kivy-webview

kivy webview这件事太头疼了,差不多大概一年前就尝试过,但是没成功,原因是.so文件
无法被识别或者无效,后面的尝试也没解决,这次搜索了许多类似的问题,感觉是环境问题
,重新撸了N遍环境,总算是有了结果.

感谢群友的鼓励和支持,特别是kivy中国开发者交流群里面的 面包大佬,闪退大佬等等...

这里要提示一下:

用pip install python-for-android似乎是不行的,这里构造的环境使用ant的旧的打包
方式,我本人从github里面安装 使用的命令是:

pip install git+https://github.com/kivy/python-for-android.git

这个成功后,环境不再使用ant来build apk,代替的是gradle,实测发现apk的体积还小了
差不多1M,可能只限于我的webview例子.

以下是环境说明:

appdirs            1.4.3  
colorama           0.3.9  
Cython             0.25.2 
docutils           0.13.1 
Jinja2             2.9.6  
Kivy               1.10.0 
Kivy-Garden        0.1.4  
MarkupSafe         1.0    
pip                18.0   
Pygments           2.2.0  
python-for-android 0.6.0  
requests           2.14.0 
setuptools         28.8.0 
sh                 1.12.0 
six                1.11.0 
wheel              0.29.0 

---------End---------------

PS:
   p4a的打包详细参数请移步查看.p4a文件.
