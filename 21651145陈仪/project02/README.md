功能：实现必选特性，太阳中心光照和tga文件纹理贴图。
平台：VS2010，OpenGl超级宝典第五版附带库：freeglut，glew和GLTools。
场景中有两个光源，一个光照照亮太阳，另一个就是以太阳为中心的光源，照亮地球和月亮。
加载tga纹理的函数是用Utility.h文件中的LoadTGA函数。其中最重要的是用GLTools库的gltReadTGABits函数。
太阳、地球、月亮纹理都贴上去了。但是有一点与第一个项目不同。glutSolidSphere函数貌似在这里不起作用，上网查了之后有人说是因为glut####画出来的都很粗糙，没有UV，所以不能贴纹理。
最后画球是用了Utility.h文件中gltDrawSphere函数。

问题：
1、抱歉，没有实现可选特性。一方面是顶点/片段着色器内容太难，上课后还不是很懂。希望老师看到了这句话后能实际操作一次。另一方面是因为最近要准备面试。请见谅。
2、因为是用了freeglut，glew和GLTools，所以在VS中要进行一系列的配置。要在VC++路径中把三个库的头文件路径包含进来，还要把三个库的lib文件放到项目下。
   不过我只上传了自己工程中的代码，所以看官要想复制粘贴编译运行的话，肯定报错一堆的哦。
