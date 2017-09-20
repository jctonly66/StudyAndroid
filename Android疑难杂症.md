1. ###问题：在开发中，有时会遇到莫名其妙的显示方面的错误，不管怎么检查都找不到错误所在，使用断点查看时程序还可能会崩溃。

     解决方法：或许是没有在主线程刷新UI。可以试试。

2. ###问题：weight、weightSum、width的使用（这里以宽为例）。
	
	解决方法：
	
	- weightSum可以指定在LinearLayout的指定方向（orientation）上weight的总份数，如果未指定，则值为所有weight加起来的大小。
	- width指定宽度，与weight一起使用时，一般设置为0dp。当然也可以设置具体的大小，此时view的宽度为：width+weight给的宽度。