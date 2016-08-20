##**俄罗斯方块**
* ***关于项目的一些注意事项***
    + 此项目由C语言编写，开发环境为VS2015（较早的版本可能会编译报错)
    + 使用了windows平台上的EGE图形库，API可以参考[EGE官网](http://xege.org)
	+ EGE官网中的安装教程都是些较老版本的IDE，VS2015可以参考 [VS2015如何导入EGE](http://www.jianshu.com/p/b12163e5a0b7)（作者已经编译好了文件直接按要求做即可）
    + 感谢您的观看  
* ***项目实现的一些功能点和具体实现方法***
    + 主要的俄罗斯方块功能
        将整个主界面分成n*m个格子(这点看你的需求)，另外一个结构体5*5矩阵存储七个方块形状(因为七个方块都是由四个小方块组成的)，非零区域表示有小方块，同理主界面也是。游戏时只要在刷新界面的时候将方块同步到主界面中就行。   
        旋转功能具体可以参考矩阵旋转九十度。  
        碰撞监测逻辑可以看blocks.cpp中的代码，很简单。
        ***游戏进行时需要记录方块左上角相对主界面的主标，下落时只改变这个坐标的纵坐标即可***
    + 背景音乐，音效
        EGE中有函数，直接调用循环播放
    + 存储用户信息
        用链表存储用户名，历史最高分数，包括排序然后返回前十名，增加用户等等
    + 其他功能
        暂停，选择关卡，重新开始
	
* ***项目素材***
	+ **方块素材**		
	![图片素材](https://github.com/Hzzone/TetrisGame/blob/master/TetrisGame/images/1.jpg?raw=true)	
	![图片素材](https://github.com/Hzzone/TetrisGame/blob/master/TetrisGame/images/2.jpg?raw=true)	
	![图片素材](https://github.com/Hzzone/TetrisGame/blob/master/TetrisGame/images/3.jpg?raw=true)	
	![图片素材](https://github.com/Hzzone/TetrisGame/blob/master/TetrisGame/images/4.jpg?raw=true)	
	![图片素材](https://github.com/Hzzone/TetrisGame/blob/master/TetrisGame/images/5.jpg?raw=true)		
	![图片素材](https://github.com/Hzzone/TetrisGame/blob/master/TetrisGame/images/6.jpg?raw=true)		
	![图片素材](https://github.com/Hzzone/TetrisGame/blob/master/TetrisGame/images/7.jpg?raw=true)		
	![图片素材](https://github.com/Hzzone/TetrisGame/blob/master/TetrisGame/images/8.jpg?raw=true)
	+	**界面素材**	
	![图片素材](https://github.com/Hzzone/TetrisGame/blob/master/TetrisGame/images/background1.jpg?raw=true)
	![图片素材](https://github.com/Hzzone/TetrisGame/blob/master/TetrisGame/images/background2.jpg?raw=true)
	![图片素材](https://github.com/Hzzone/TetrisGame/blob/master/TetrisGame/images/background3.jpg?raw=true)
	![图片素材](https://github.com/Hzzone/TetrisGame/blob/master/TetrisGame/images/gameover.jpg?raw=true)	
	![图片素材](https://github.com/Hzzone/TetrisGame/blob/master/TetrisGame/images/background4.JPG?raw=true)
* ***项目效果图***	

