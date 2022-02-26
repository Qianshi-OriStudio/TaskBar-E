##########README##########
StackBlur是什么？
StackBlur.js 是 Mario Klingemann 创建的一个快速的、接近高斯模糊的效果库.
StackBlur.js最著名的移植项目是Android StackBlur
这个库能够基于渐变或radius对一个Bitmap进行模糊化处理


软件中合适的附带模糊效果能让软件拥有更好的视觉效果，同时也能让用户将注意力从花哨的背景转到关注软件本身上。

目前网上开源的模糊库大多重复，而实现原理很多都是gdi，先不说效率问题，就说gdi中的模糊函数，是在win7之后加入的，也就是说只支持win7以上(好像win8的模糊函数也被隐藏了)。

StackBlur是直接对图像的内存进行操作，修改内存比特来实现模糊算法，这便提高了处理速度，并且兼容性与扩展性也大大提高。
网上有个StackBlur的编译好的版本，效率很高(需要附加一个NVIDIA的硬件加速库能不快吗)，与之一起的是体积较大  

本版本是从开源的多线程版StackBlur-c++移植过来（删掉了多线程库就成了纯C），编译后大小只有13K

出处: https://bbs.125.la/forum.php?mod=viewthread&tid=14545186