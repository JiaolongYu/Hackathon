# Hackathon
intern hackathon

Game Name: Gocha
              ________
             /        \ 
       ()() /       o  \ 
        \ \_\       ~~ /
         \____________/ 

Init page:
________________________________________
|										|
|										|
|										|
|										|
|			logo & game name			|
|										|
|										|
|		 ______________________ 		|
|		|					   |		|
|		|	one player mode	   |		|
|		|______________________|		|
|										|
|		 ______________________ 		|
|		|				   	   |		|
|		|	  battle mode      |		|
|		|______________________|		|
|										|
|		 ______________________ 		|
|		|					   |		|
|		|	  score board	   |		|
|		|______________________|		|
|										|
|		 ______________________ 		|
|		|					   |		|
|		|	    settings   	   |		|
|		|______________________|		|
|										|
|										|
|								    	|
|										|
|								 ___	|
|								/	\   |
|username			  (login)   \___/	|
|version						    	|
|_______________________________________|

（我们没有厂标和初始画面之类的，所以直接放logo和title在最上面。一般初始页面需要显示用户名和游戏版本号，通常在右下角， 但是如果放一个login同样在右下角的话好像看上去有点奇怪，所以版本号和用户名放左下角了。）
（设定页面待定。一般有音效ON OFF，按键音ON OFF，动画效果ON OFF，音量大小调整）
私心：菜单按钮也都做成鱼的形状，圆的登陆按钮做成泡泡，感觉会比较萌

one player mode：
画面参照学长找到的那个灵感视频（求截图发群里
________________________________________
|								   __	|
|                                 /  \  |
|	level:  1	score:    10	 ( || )	|
|                                 \__/  |
|	 ______________	  ______________	|
|	|			   | |				|	|
|	|			   | |				|	|
|	|			   | |				|	|
|	|			   | |				|	|
|	|			   | |		    	|	|
|	|			   | |				|	|
|	|			   | | 				|	|
|	|			   | |				|	|
|	|			   | |				|	|
|	|	 		   | |				|	|
|	|			   | |				|	|
|	|			   | |				|	|
|	|			   | |				|	|
|	|			   | |				|	|
|	|			   | |				|	|
|	|			   | |				|	|
|	|			   | |		    	|	|
|	|			   | |				|	|
|	|			   | | 				|	|
|	|			   | |				|	|
|	|			   | |				|	|
|	|	 		   | |				|	|
|	|			   | |				|	|
|	|			   | |			    |	|
|	|			   | |				|	|
|	|______________| |______________|	|
|									    |
|username			  					|
|version						    	|
|_______________________________________|
上方有显示难度等级和积分，（泡泡状）暂停键，按下后游戏暂停，屏幕中央产生子菜单：Continue 和 Quit
左道吃鱼，右道被鱼吃
每边2道，按照点击屏幕换左右方向，点击左下半屏幕作为左边换道操作，点击右下半屏幕作为右边换道操作（3道？手指移动控制换向？）
难度等级按照难度系数分级自动更新，积分自动更新

数值设定（暂定）
积分 ＝ 掉落数量 ＊ 10
游戏难度系数 ＝ 积分 ＊ 比例因子1
暂时用于调整掉落间隔时间和掉落速度
掉落间隔时间 ＝ 0.5s － 难度系数 ＊ 比例因子2
掉落速度 ＝ 20pix／s ＋ 难度系数 ＊ 比例因子3

吃到以及被吃判定（暂定）
接触即算，被吃或没吃到游戏结束，分数更新到本地积分榜。吃到则掉落的鱼立即消失，没有碰到大鱼即大鱼消失
（难度大可试换EASY：以被吃作为游戏结束与否判定，吃到作为积分奖励但失败不导致游戏结束）

two players mode：
进入后还要先做玩家匹配，界面待定，匹配完成后进入游戏。
游戏界面和单人模式相比无暂停。游戏结束屏幕中央弹出Win或Loss以及菜单键Another game和Quit
（这部分我和网易的同学讨论了一下，因为互扔道具这个设定对于玩家来说，如果在屏幕上看不到扔道具的效果的话意义不大，但是画面不适合再加一个对手画面，所以更改设定如下）
只对吃鱼的左边进行和单人模式一样的掉落和积分，一旦玩家吃到一条鱼，就在对方玩家的右边躲避上刷新一条大鱼，相当于左手给对方加障碍，右手躲避对方所给的障碍。
任意一边先出错则输。

