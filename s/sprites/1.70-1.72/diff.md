# Comparing `tmp/sprites-1.70.tar.gz` & `tmp/sprites-1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprites-1.70.tar", last modified: Mon May 29 09:32:11 2023, max compression
+gzip compressed data, was "sprites-1.72.tar", last modified: Wed Jun 21 07:38:40 2023, max compression
```

## Comparing `sprites-1.70.tar` & `sprites-1.72.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 09:32:11.152691 sprites-1.70/
--rw-rw-rw-   0        0        0     2099 2023-05-29 09:32:11.150691 sprites-1.70/PKG-INFO
--rw-rw-rw-   0        0        0     1001 2023-05-29 09:32:05.000000 sprites-1.70/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 09:32:11.154692 sprites-1.70/setup.cfg
--rw-rw-rw-   0        0        0     1306 2023-05-29 09:30:55.000000 sprites-1.70/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 09:32:11.114689 sprites-1.70/sprites/
--rw-rw-rw-   0        0        0  1438345 2023-05-29 06:20:09.000000 sprites-1.70/sprites/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 09:32:11.144691 sprites-1.70/sprites.egg-info/
--rw-rw-rw-   0        0        0     2099 2023-05-29 09:32:10.000000 sprites-1.70/sprites.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-29 09:32:11.000000 sprites-1.70/sprites.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 09:32:10.000000 sprites-1.70/sprites.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-29 09:18:17.000000 sprites-1.70/sprites.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-05-29 09:32:10.000000 sprites-1.70/sprites.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-29 09:32:10.000000 sprites-1.70/sprites.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 07:38:40.607067 sprites-1.72/
+-rw-rw-rw-   0        0        0     2099 2023-06-21 07:38:40.606067 sprites-1.72/PKG-INFO
+-rw-rw-rw-   0        0        0     1001 2023-05-29 09:32:05.000000 sprites-1.72/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-21 07:38:40.611068 sprites-1.72/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-06-21 07:38:25.000000 sprites-1.72/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:38:40.536063 sprites-1.72/sprites/
+-rw-rw-rw-   0        0        0  1439652 2023-06-21 07:37:56.000000 sprites-1.72/sprites/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 07:38:40.595067 sprites-1.72/sprites.egg-info/
+-rw-rw-rw-   0        0        0     2099 2023-06-21 07:38:40.000000 sprites-1.72/sprites.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-06-21 07:38:40.000000 sprites-1.72/sprites.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 07:38:40.000000 sprites-1.72/sprites.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-21 07:38:34.000000 sprites-1.72/sprites.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-06-21 07:38:40.000000 sprites-1.72/sprites.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-21 07:38:40.000000 sprites-1.72/sprites.egg-info/top_level.txt
```

### Comparing `sprites-1.70/PKG-INFO` & `sprites-1.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprites
-Version: 1.70
+Version: 1.72
 Summary: Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类等及一些工具函数,如洪水填充命令,几何相关命令。它支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。微信:scratch8，专业编程私教。网址： www.lixingqiu.com
 Home-page: http://www.lixingqiu.com
 Author: lixingqiu
 Author-email: 406273900@qq.com
 License: MIT
 Description: ﻿# Python sprites module introduce
```

### Comparing `sprites-1.70/README.md` & `sprites-1.72/README.md`

 * *Files identical despite different names*

### Comparing `sprites-1.70/setup.py` & `sprites-1.72/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding='utf-8') as fh:
     long_d = fh.read()
 
 
 setup(name='sprites',
       long_description_content_type="text/markdown",
-      version = '1.70',
+      version = '1.72',
       description = 'Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类等及一些工具函数,如洪水填充命令,几何相关命令。它支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。微信:scratch8，专业编程私教。网址： www.lixingqiu.com',
       long_description = long_d,      
       keywords = 'creative game pygame turtle animation sprite geometry math Elementary Mathematics Teaching',
       url = 'http://www.lixingqiu.com',
       wechat = 'scratch8',
       author ='lixingqiu',
       author_email = '406273900@qq.com',
```

### Comparing `sprites-1.70/sprites/__init__.py` & `sprites-1.72/sprites/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
    3. onscreenrelease：鼠标松开事件，需要定义一个函数绑定它。
    4. move：在水平和垂直方向上移动背景图片。
    5. setx：设置背景图片的x坐标。
    6. sety：设置背景图片的y坐标。
    7. xcor：获取背景图片的x坐标。
    8. ycor：获取背景图片的y坐标。
    9. goto：设定背景图片的x,y坐标
-   10. save：截屏，保存屏幕为图形对象或者为图片，屏幕需在最前面显示(不要最小化)。
+   10.capture: 别名是save,用于截屏，保存屏幕为图形对象或者为图片，屏幕需在最前面显示(不要最小化)。
    11. titlebar：是否要标题栏的命令，参数为False，不显示标题栏，反之显示。
    12. draggable：让窗口按住鼠标中键时可拖动。在没有标题栏时最好这样，要不然不方便了。
    13. addpopup：绑定右键菜单
    14. removepopup：移除绑定右键菜单
    15.inputbox函数,用于输入对话框
    16.hide 隐藏窗口
    17.show 显示窗口
@@ -177,15 +177,15 @@
    原因是绑定盒命令得到的是先前没有刷新的角色的坐标，这样获取的不是最新坐标，当然会导致程序出意外。
    4. 屏幕的update命令会重新渲染所有的角色，如果角色较多，反而会让程序运行更慢。
    5. 本模块给RawTurtle类增加了update方法，这样能单独渲染一个角色。本模块已经把屏幕的自动绘画延时设为0及速度也设为最快了。
    6. 其实Turtle模块可以支持png图片,但要像以下这样写:
    screen.addshape('scratch.png',Shape("image", screen._image('scratch.png')))
 """
 __author__ = 'lixingqiu'
-__date__ = '2023/5/29'
+__date__ = '2023/06/21'
 __blog__ = 'www.lixingqiu.com'
 
 import os
 import re
 import sys
 import math
 import glob
@@ -199,15 +199,15 @@
 from copy import deepcopy
 from tkinter import filedialog
 from tkinter import colorchooser
 from winsound import PlaySound,SND_ASYNC,SND_LOOP,SND_PURGE
 from PIL import ImageTk,ImageOps,Image,ImageGrab,ImageDraw,ImageFont,ImagePath,ImageColor
 from turtle import TK,_Root,ScrolledCanvas,_CFG ,TNavigator,Tbuffer,TPen,_Screen,Screen,Turtle,Vec2D, RawTurtle,TurtleScreenBase,Shape,TurtleScreen,_TurtleImage,TurtleGraphicsError 
 
-_VERSION = 1.70 
+_VERSION = 1.72 
 _CFG['delay'] = 0
 # 定义资源文件夹
 _resfld = os.path.join(os.getcwd(),'res')
 if not os.path.exists(_resfld):os.mkdir(_resfld)
 
 class InputBox:
     def __init__(self,master,title='输入对话框',prompt='请输入字符:'):
@@ -275,18 +275,20 @@
     def show_textmenu(self,event):
         e_widget = event.widget
         self.the_menu.entryconfigure("剪切",command=lambda: e_widget.event_generate("<<Cut>>"))
         self.the_menu.entryconfigure("复制",command=lambda: e_widget.event_generate("<<Copy>>"))
         self.the_menu.entryconfigure("粘贴",command=lambda: e_widget.event_generate("<<Paste>>"))
         self.the_menu.entryconfigure("全选",command=lambda: e_widget.select_range(0, 'end'))
         self.the_menu.tk.call("tk_popup", self.the_menu, event.x_root, event.y_root)
-    
-    
+        
 def makerndfilename(ext=''):
-    """生成随机文件名,ext是扩展名,如.png """
+    """生成随机文件名,
+    参数: ext表示扩展名,如.png
+    举例:fn = makerndfilename('.txt')
+    """
     s = 'abcdefghijklmnopqrstuvwxyz0123456789'
     t = time.localtime()
     year = str(t.tm_year)
     mon = str(t.tm_mon)
     day = str(t.tm_mday)
     minu = str(t.tm_min)
     sec = str(t.tm_sec)
@@ -374,23 +376,25 @@
 def _redef_setupcanvas(self, width, height, cwidth, cheight):
     self._canvas = ScrolledCanvas(self.displayframe, width, height, cwidth, cheight)
     self._canvas.pack(side=TK.LEFT,expand=1,fill='both')
 _Root.setupcanvas = _redef_setupcanvas
 
 # 给root增加position获取坐标方法,注意坐标系是右下为正的
 def _Rootposition(self):
+    """返回窗口的坐标"""
     string = self.geometry()
     info = string.split('+')
     left = int(info[1])
     top = int(info[2])
     return left,top
 _Root.position= _Rootposition
 
 # 给root增加goto坐标定位方法,注意坐标系是右下为正的
 def _Rootgoto(self,x,y):
+    """让窗口到达某个坐标"""
     string = "+" + str(x) + "+" + str(y)    
     self.geometry(string)
 _Root.goto = _Rootgoto
   
 # 给root增加move方法,
 def _Rootmove(self,dx,dy=0):
     """窗口的移动方法,注意坐标系是右下为正的"""
@@ -504,15 +508,16 @@
 
     self._update() #count=True)
 RawTurtle._goto = RawTurtle_goto
 
 
 # 给原生海龟增加slide，别名glide方法
 def RawTurtle_slide(self,pos,delay=2000):
-    """pos：x,y坐标,元组或者列表,如果不是这两个,则先处理一下
+    """滑行到某个坐标点. 
+       pos：x,y坐标,元组或者列表,如果不是这两个,则先处理一下
        delay：以毫秒为单位的滑行总时间
        在规定的时间内滑动到坐标，无返回值。
     """
     # 处理pos不是列表或者元组的情况
     if not isinstance(pos,(tuple,list)):# 不是列表或者元组,当成当x值
         pos = (pos,self.ycor())
     
@@ -536,15 +541,15 @@
     self.screen.delay(old_delay)
     
 RawTurtle.slide = RawTurtle_slide
 RawTurtle.glide = RawTurtle_slide
 
 # 给原生海龟增加update方法，为的是能单独渲染一个角色
 def RawTurtle_update(self):
-    """重画自己"""
+    """重新刷新对象"""
     tracing = self.screen._tracing
     self.screen._tracing = True
     self._update_data()
     self._drawturtle()
     self.screen._update()
     self.screen._tracing = tracing
 RawTurtle.update = RawTurtle_update
@@ -597,15 +602,15 @@
             for item in titem:
                 screen._drawpoly(item, ((0, 0), (0, 0), (0, 0)), "", "")
         self._hidden_from_screen = True
 RawTurtle._drawturtle = RawTurtle_drawturtle
             
 # 给原生海龟对象增加move方法
 def _move(self,dx=0,dy=0):
-    """移动水平dx,垂直dy的距离"""
+    """在水平和垂直方向移动dx及dy个单位"""
     x = self.xcor() + dx
     y = self.ycor() + dy
     self.goto(x,y)
     self._update()
 RawTurtle.move = _move
 
 # 给原生海龟增加stop方法,用于停止播放音乐
@@ -794,35 +799,31 @@
 TurtleScreen.setalpha = TurtleScreen_setalpha
 
 # 给TurtleScreen添加finditems方法
 def TurtleScreen_finditems(self):
     """查找所有可用于碰撞检测的items,包括线条lineitem,_fillitem,polyitem"""
     rs = [None,(-3, -3, 3, 3),(-1, -1, 1, 1),(0, 0, 1, 1)]
     items = self.cv.find_all()       # 所有items    
-    items = list(items)
-     
-    items.remove(self._bgpic)        # self._bgpic是背景图的item编号
-    
+    items = list(items)     
+    items.remove(self._bgpic)        # self._bgpic是背景图的item编号    
     # 把说话泡泡的items也去掉
     tbitems = []                     # 保存所有说话泡泡的items
     tbs = [tu._draw_bubble_turtle for tu in self._turtles if tu._tag=='sprite']
     [tbitems.extend(tb.items) for tb in tbs]   
     [items.remove(item) for item in tbitems]
-
     # 下面是把一些预定义的item去掉
     for item in items[:]:
       bbox = self.cv.bbox(item)
-      if bbox in rs:items.remove(item)
-    
+      if bbox in rs:items.remove(item)    
     return items
 TurtleScreen._finditems = TurtleScreen_finditems
     
 # 给TurtleScreen添加setcover方法
 def TurtleScreen_setcover(self):
-    """ 去除标题栏等"""
+    """ 去除标题栏等,当把窗口当成封面时可调用这个方法."""
     bgcolor= self._root._canvas._canvas["bg"]
     self._root.overrideredirect(1)               # 去除标题栏
     self._root._canvas._canvas.configure(highlightthickness=0)
     self._root._canvas._canvas.configure(borderwidth=0)
     # 下面这个_canvas是继承自frame的一个组件
     self._root._canvas.configure(bg=bgcolor)
     self._root._canvas.configure(highlightthickness=0)
@@ -864,15 +865,15 @@
    if eventfun is None:
       self.cv.unbind("<KeyPress>", None)
    else:
       self.cv.bind("<KeyPress>", eventfun)
 TurtleScreen.onanykey = TurtleScreen_onanykey
 
 def TurtleScreen_xy_grid(self,colorindex=0,step=100):
-    """画直角坐标格子图"""
+    """显示平面直角坐标系,即画直角坐标格子图"""
     linecolors = ['gray90','gray20']     # 线条颜色 
     xaxiscolors = ['orange','#4D0505']     # x轴颜色
     yaxiscolors = ['#0000C6','#063167']  # y轴颜色
     xtextcolors =['orange','#614804']
     ytextcolors =['#C5C3FF','#094277']   # y,那个100的文字颜色
     
     width = self.cv.winfo_width()
@@ -931,20 +932,19 @@
 
 TurtleScreen.rt_grid = TurtleScreen_rt_grid
 TurtleScreen.polar_grid = TurtleScreen_rt_grid
 
 
 # 新增屏幕保存方法,保存的是截取的图形
 def TurtleScreen_save(self,filename=None,size=None,margin=5,full=False):
-    """ 截屏命令，能截精灵所在的窗口的屏幕或者电脑桌面全屏与指定矩形区域。
-        filename:截屏后要保存的图像文件名,推荐用png,不写文件名则返回im图形对象。      
+    """ 截屏命令，能截角色所在的窗口的屏幕或者电脑桌面全屏与指定矩形区域。
+        filename:截屏后要保存的图像文件名,推荐用png,不写文件名则返回pillow图形对象。      
         size:截屏区域,四元组,表示左上角和右下角坐标，如果指定了size，那么margin参数不起作用。
         margin:左上角与右下角边距。
-        full: 表示是否全屏截取，如果指定了full为True，那么size和margin参数不起作用。
-        
+        full: 表示是否全屏截取，如果指定了full为True，那么size和margin参数不起作用。        
     """
     if full == True:
        im = ImageGrab.grab()
     else:
        if size == None:
          c = Turtle._screen._root._canvas  # 获取画布对象
          x0 = c.winfo_rootx() + margin     # 画布左上角x坐标
@@ -962,14 +962,15 @@
        im = ImageGrab.grab(size)
     if filename == None:
        return im
     else:
        im.save(filename)
       
 TurtleScreen.save = TurtleScreen_save
+TurtleScreen.capture = TurtleScreen_save
   
 def _Screen__init__(self,layout=1):
       """新建一个窗口,如果存则,什么也不干,layout是新增的布局参数"""
       if _Screen._root is None:
           # 下面这样做的原因是在实际开发中如果在程序中重定义Root类,
           # 如果没有参数那会出错,为了兼容,所以用了try
           try:
@@ -1358,42 +1359,42 @@
         tmppic = Image.open(tmppic)
         #tmppic.save(os.path.join(_resfld,_built_in_images[i]))        
         tmppic.show()
         tmppic.close()
     else:
         input("查无结果")
 
-
 # 几何相关的独立函数2022年9月
 def three_point_order(A,B,C):
-    """判断三点顺序，逆时针或者顺时针，亦可用于判断三点是否共线"""
+    """判断三点顺序，逆时针或者顺时针，亦可用于判断三点是否共线，
+       返回值大于0表示三点逆时钟顺序，小于0表示顺时钟，等于0表示三点共享。"""
     x1,y1 = A
     x2,y2 = B
     x3,y3 = C
     r = (x2-x1)*(y3-y1)-(y2-y1)*(x3-x1)
     # r大于0，逆时钟，r<0顺时针，r==0共线
     return r
 
 def pick_point(A,C,k=2):  # 在经过A和C点的直线上取点
     """在经过A和C点的直线上取点。
        A是个点,C是个点,以二元组表示,假设它们之间的点叫D,则k是AD/DC的比值
-       这个函数根据k的大小求D的坐标.
+       这个函数根据k的大小返回D的坐标.
     """
     x1,y1 = A;x2,y2 = C
     x = (x1 + k*x2) / (k+1)
     y = (y1 + k*y2) / (k+1)
     return x,y
 pickpoint = pick_point
 
 def midpoint(p1,p2):
     """返回p1,p2之间的中点"""
     return pick_point(p1,p2,1)
 
 def twopointoneline(p1,p2):
-    """两点一线函数，
+    """两点一线函数，根据两个点返回直线方程的系数。
     p1,p2表示坐标点,用二元组表示,本函数根据两点返回一元一次方程一般式的A,B,C,k,b"""
     x1,y1 = p1
     x2,y2 = p2
     dx = x1 - x2
     if dx==0:
         k = b = float('inf')
     else:
@@ -1451,28 +1452,27 @@
         if y>y2 or y<y1 : return False
         return True
     else:
         return False
 dot_is_on_segment = point_is_on_segment
 
 def is_collinear(A,B,C):
-    """三点共线"""
+    """判断三点是否共线"""
     line = B,C
     return point_is_on_line(A,line)
     
 def segment_intersection(segment1,segment2):
     """返回两条线段的交叉点
        segment:两个点表示的线段,如((10,10),(20,20))或[(0,0),(100,100)]
     """
     jiaodian = line_intersection(segment1,segment2)   # 直线1和直线2的交点
     if jiaodian==None:return None
     if point_is_on_segment(jiaodian,segment1) and point_is_on_segment(jiaodian,segment2):
         x,y  = jiaodian
-        return x,y
-    
+        return x,y    
     
 def lc_intersection(line,circle):  # 直线与圆的交点
     """返回直线和圆的交点  
        line是用两点表示的直线,形如,((32,99),(0,0))或[(32,99),(0,0)]
        circle: 用圆心和半径表示的圆形，如[(0,0),100]，表示圆心在原点，半径为100的圆
     """
     if isinstance(circle,dict):
@@ -1526,16 +1526,15 @@
 def is_on_circle(point,circle):
     """判断点是否在圆上
        point:用二元组表示的点,circle:中心点与半径表示的圆,如((0,0),100)"""
     if isinstance(circle,dict):
         radius,center = circle.popitem()        # 弹出项目，此时字典已空
     else:
         center = circle[0]                 # 取出圆心
-        radius = circle[-1]                # 取出半径
-    
+        radius = circle[-1]                # 取出半径    
     a,b = center
     x,y = point
     # 下面根据圆的标准方程判断x,y是否在圆上
     return  (x-a)**2 + (y-b)**2 == radius**2 
 point_is_on_circle = is_on_circle
 dot_is_on_circle = is_on_circle
 
@@ -1577,15 +1576,15 @@
         y2 = y + A * (b-y)/d
         x3 = x2 - h * (b - y) / d
         y3 = y2 + h * (a - x) / d
         x4 = x2 + h * (b - y) / d
         y4 = y2 - h * (a - x) / d
         return [(x3,y3),(x4,y4)]
     
-def __intersection_bak(item1,item2,combmode=0):   #  不要用这个函数，已废 
+def __intersection_bak(item1,item2,combmode=0): # 不要用这个函数，已废 ，留尸而已
     """两个对象相交，仅支持点，直线，线段与圆
        item1与item2可表示：点，直线、线段、圆。
        本函数严格区分点，线段，直线的表示方法，我们默认以下规则：
        1.用二元组表示一个点，如(0,0)表示原点
        2.用在列表中的两个点表示线段，如[(0,0),(10,10)]表示从原点到(10,10)的线段。
        3.用在元组中的两个点表示经过两点的直线，如((0,0),(10,10))表示经过这两个点的直线。
        4.用点和半径表示圆，并用中括号括起来，如[(0,0),100]
@@ -1692,59 +1691,60 @@
     elif mode==8:return point_is_on_segment(item1,item2)    # 点是否在线段上
     elif mode==9:return is_on_circle(item1,item2)           # 点是否在圆上
     
 intersect = intersection          # 取别名     
 
     
 def symmetric_points(points,center):          # 中心对称
-    """中心对称,一些点关于center对称,返回对称的点"""
+    """中心对称,一些点关于center对称,返回列表，此列表中包括所有对称的点"""
     p1 = np.array(points)
     c = np.array([center])
     p2 = 2*c - p1
     p2 = [(x,y) for x,y in p2]
     return p2
 
 def perpendicular_foot(p,line):
-    """返回p点关于直线的垂足点,p:二元组表示的坐标点,line:有两个二元组的列表,如[(0,0),(100,100)]"""
+    """返回p点关于直线的垂足点,
+       p:二元组表示的坐标点,line:由两个二元组形成的列表,如[(0,0),(100,100)]"""
     A2,B2,C2,k,b = twopointoneline(*line)#直线一般式的5个参数
     if k==0:
         A1=1;B1=0;C1=p[0]
         x = p[0];y=b
     else:
         A1,B1,C1 = kpointoneline(p,-1/k)#通过一点和斜率确定直线
         m = A1*B2 - A2*B1
         if m==0:return None
         x = (C2*B1-C1*B2)/m    #  交点(垂足点)
         y = (C1*A2-C2*A1)/m
     return x,y 
 
 def axis_points(points,line):            # 轴对称
-    """本函数求一些点关于直线line的对称点"""
+    """本函数求一些点关于直线line的轴对称点，返回一个列表"""
     p1,p2 = line
     A,B,C,*x = twopointoneline(p1,p2)
     rp = []
     def f(p,A,B,C):
         x,y = p
         t = (A*x+B*y+C)/(A*A+B*B)
         x = x - 2*A*t
         y = y - 2*B*t
         return x,y
-    rp = [f(p,A,B,C) for p in points]
-     
+    rp = [f(p,A,B,C) for p in points]     
     return rp
 
 def homothetic_points(points,center,k):          # 位似
-    """位似的多个点:points,center:位似心中心,k:位似比"""
+    """返回位似的多个点，
+       points:坐标点,center:位似心中心,k:位似比"""
     c = center    
     return [(k*(c[0]-dot[0])+c[0],k*(c[1]-dot[1])+c[1])
             for dot in points]
 dilate = homothetic_points
 
 def is_same_direction(center,p,cor,k):
-    """反演中心:center,p:待反演的点,cor:已经反演的点,k反演幂"""
+    """center：反演中心,p:待反演的点,cor:已经反演的点,k反演幂"""
     O = Vec2D(*center)
     OA = Vec2D(*p) - O
     OA_ = Vec2D(*cor) - O
     return np.sign(OA*OA_)==np.sign(k)
     
 def inverting_points2_(points,center,k):          # 反演
     """本人算法,暂时不用以作纪念,反演的多个点:points,center:位似心中心,k:反演常数"""
@@ -1794,16 +1794,17 @@
         jiao = 0
     else:
         k = (c*c + a*a - b*b)/(2*a*c)
         jiao = math.degrees(math.acos(k))
     if three_point_order(A,B,C)<0:jiao = 360-jiao  # 如果三点是顺时针
     return jiao
     
-def angle_bisector(A,B,C): # 使用角平分线定理求角平分线和对边的交点
-    """A,B,C是三个以二元组表示的点，求角平分线,返回从B点出发的角平分线和AC的交点"""
+def angle_bisector(A,B,C): # 角平分线
+    """使用角平分线定理求角平分线和对边的交点，
+       A,B,C是三个以二元组表示的点，求角平分线,返回从B点出发的角平分线和AC的交点"""
     a = BC = math.dist(B,C)
     b = AC = math.dist(A,C)
     c = AB = math.dist(A,B)
     k = c/a
     return pick_point(A,C,k)
 
 def perpendicular_bisector(segment,length=100): # 中垂线
@@ -1825,15 +1826,15 @@
      t = Pointer(pos=p1)
      j = t.towards(p2)
      t.setheading(j)
      t.goto(p);t.fd(length/2);dot1=t.position()
      t.bk(length);dot2 = t.position()
      return dot1,dot2    
 
-def circle_on_tangent(circle,point,length=100):
+def circle_on_tangent(circle,point,length=100): # 圆上切线 
     """圆上的切线,默认长度100),返回两个点
        circle：圆形，用[(0,0),100]这样的数据表示一个圆
        point：点，用二元组表示的点，如(10,10)
     """
     if isinstance(circle,dict):
         radius,center = circle.popitem()        # 弹出项目，此时字典已空
     else:
@@ -1841,15 +1842,15 @@
     p = point
     t = Pointer(pos=center)
     j = t.towards(p);t.setheading(j)
     t.fd(radius); t.left(90);t.fd(length/2);dot1 = t.position()
     t.bk(length);dot2 = t.position()
     return dot1,dot2
 
-def circle_out_tangent(circle,point):
+def circle_out_tangent(circle,point):   # 圆外切线
     """圆外一点到圆的两条切线,返回两个点
        circle：圆形，用[(0,0),100]这样的数据表示一个圆
        point：点，用二元组表示的点，如(10,10)
     """
     if isinstance(circle,dict):
         radius,center = circle.popitem()        # 弹出项目，此时字典已空
     else:
@@ -1901,16 +1902,15 @@
     """圆外随机点
        circle：是形如[(10,10),100]这样的数据，列表中的数据表示圆心和半径
     """
     if isinstance(circle,dict):
         radius,center = circle.popitem()        # 弹出项目，此时字典已空
     else:
         center = circle[0]                 # 取出圆心
-        radius = circle[-1]                # 取出半径 
-
+        radius = circle[-1]                # 取出半径
     t = Pointer(pos=center)
     angle = random.randint(1,360)
     t.setheading(angle)
     d = radius + radius*random.uniform(*limits)
     t.fd(d);dot = t.position()
     return dot
 
@@ -1946,15 +1946,14 @@
         distance:要移动的距离,angle:移动的方向值
     """
     a = math.radians(angle)
     dx = distance*math.cos(a)
     dy = distance*math.sin(a)
     return move_points2(cors,dx,dy)
 
-
 def convert_cross_xy(points):
     """把坐标转换成以图像左上角为原点的,points是列表,存储一些坐标点"""
     min_x = min([x for x,y in points])
     max_x = max([x for x,y in points])
     width = max_x - min_x
     center_x  = (min_x+max_x)/2
     min_y = min([y for x,y in points])
@@ -1977,15 +1976,15 @@
     size = size[0]+1,size[1]+1
     img = Image.new("RGBA", size)  
     img1 = ImageDraw.Draw(img)   
     img1.polygon(points, fill=fill, outline =outline)  
     return img ,center
 
 def make_rect_image(length,height,fill=(198,155,25,128),outline=None):
-    """产生矩形图像"""    
+    """产生矩形图像，返回pillow图形对象。"""    
     A = (0,0)               # 左下角坐标
     B=(length-1,0)          # 右下角坐标
     C=(length-1,height-1)   # 右上角坐标
     D=(0,height-1)          # 左上角坐标
     im,_ = poly2image([A,B,C,D],fill=fill,outline=outline)
     return im
 
@@ -1996,27 +1995,30 @@
     size = w,h
     im = Image.new("RGBA",size,(0,0,0,0)) # 新建RGBA格式无色图
     draw = ImageDraw.Draw(im)
     draw.ellipse((0,0,w-1,h-1),fill=fill)
     return im    
 
 def centroid(A,B,C):         # 重心,三条中线交点
+    """返回三角形的重心,中线交点"""
     return (A[0]+B[0]+C[0])/3,(A[1]+B[1]+C[1])/3
 
 def incenter(A,B,C):         # 内心,三条角平分线的交点
+    """返回三角形的内心，角平分线交点"""
     x1,y1 = A
     x2,y2 = B
     x3,y3 = C
     BC = a = math.dist(B,C)
     CA = b = math.dist(C,A)
     AB = c = math.dist(A,B)
     p = a + b + c
     return (a*x1+b*x2+c*x3)/p,(a*y1+b*y2+c*y3)/p
 
 def excenter(A,B,C):         # 外心,三条中垂线的交点
+    """返回三角形的外心，垂直平分线交点"""
     x1,y1 = A
     x2,y2 = B
     x3,y3 = C
     A1 = 2*(x2-x1)
     B1 = 2*(y2-y1)
     C1 = x2*x2+y2*y2-x1*x1-y1*y1
     A2 = 2*(x3-x2)
@@ -2025,14 +2027,15 @@
     P = (A1*B2-A2*B1)
     x = (C1*B2-C2*B1) / P
     y = (A1*C2-A2*C1) / P
     return x,y
 circumcenter = excenter
 
 def orthocenter(A,B,C):         # 垂心,三条高的交点
+    """返回三角形的垂心，三条高的交点"""
     x1,y1 = A;    x2,y2 = B;    x3,y3 = C    
     BC = a = math.dist(B,C)
     CA = b = math.dist(C,A)
     AB = c = math.dist(A,B)
     cosA = (b*b + c*c - a*a)/(2*b*c)
     if cosA==0:return A
     aA = a/cosA
@@ -2112,27 +2115,27 @@
 
 
 def heron_formula(A,B,C):
     """运用海伦公式求三角形面积，A，B，C是三个不共线的坐标点
     """
     a = math.dist(B,C);b = math.dist(A,C);c = math.dist(B,A)
     p = (a+b+c)/2
-    return (math.sqrt(p*(p-a)*(p-b)*(p-c)),p )         # 注意返回的是面积与周长的一半
+    return (math.sqrt(p*(p-a)*(p-b)*(p-c)),p ) # 注意返回的是面积与周长的一半
     
 def circumcircle(A,B,C):              # 三点定圆
     """返回外接圆,A,B,C是不共线的三个点"""
     a = math.dist(B,C);b = math.dist(A,C);c = math.dist(B,A)
     p = (a+b+c)/2
     s = math.sqrt(p*(p-a)*(p-b)*(p-c))
     r = a*b*c/(4*s)
     return (circumcenter(A,B,C),r)
 
 def incircle(A,B,C):
     """返回内切圆,A,B,C是不共线的三个点"""
-    s,p = heron_formula(A,B,C)
+    s,p = heron_formula(A,B,C)  # 返回的三角形面积和周长的一半
     r = s/p
     return (incenter(A,B,C),r)
 
 def inflection_points(polyline):
     """返回折线的拐点,polyline是一个点集，如[(0,0),(10,10),(20,20),(20,30)]"""
     points = polyline
     guaidians = []
@@ -2490,16 +2493,15 @@
     y1 = y0 + 0.5 * height * scale
     x2 = x0 + 0.5 * width * scale
     y2 = y0 - 0.5 * height * scale
 
     return x1,y1,x2,y2
   
 # 产生一个颜色表，里面的颜色较鲜艳
-def makecolors(n=128):
-        
+def makecolors(n=128):        
     """产生颜色表，饱和度和亮度最高，所以很鲜艳"""
     cs = []
     for y in range(n):
         x = random.random()
         r,g,b = colorsys.hsv_to_rgb(x,1,1)
         r,g,b = int(r*255),int(g*255),int(b*255)
         cs.append((r,g,b))
@@ -2546,15 +2548,15 @@
         return time.perf_counter() - self._old_start_time
     
     def getfps(self):
         """得到fps"""
         t = time.perf_counter() - self._old_start_time
         return round(1/t,2)
 
-def rect_overlap(rect1,rect2):
+def rect_overlap(rect1,rect2): # 矩形重叠
     """
         rect1：矩形1，四元组，左上角坐标和右下角坐标
         rect2：矩形2，四元组，左上角坐标和右下角坐标
         本函数返回矩形相交区域的矩形及面积
     """
     (x11,y11,x12,y12) = rect1     # 矩形1左上角(x11,y11)和右下角(x12,y12) 
     (x21,y21,x22,y22) = rect2     # 矩形2左上角(x21,y21)和右下角(x22,y22)
@@ -2767,15 +2769,15 @@
     """      
     def __init__(self,shape=os.path.join(_resfld,'bug.png'),
                  pos=(0,0) ,visible=True,
                  undobuffersize=_CFG["undobuffersize"],tag='sprite',heading=0):
         """
            shape：造型图像(int或str)，pos：起始坐标，visible：可见性，
            undobuffersize：可撤销次数,tag:标签,heading:初始方向。
-           新建一个精灵，默认为小虫子，在屏幕中央。
+           新建一个角色，默认为小虫子，在屏幕中央。
         """
         self._id = str(id(self))                        # 唯一标识
         self._initend = False                           # 表示初始化开始
         Turtle.__init__(self,visible=False,undobuffersize=undobuffersize,shape='blank')
         self._stampcors = { }                           # 记录每个图章坐标的字典，键为图章编号 
         self._rotatemode = 0                            # 设定旋转模式，0:360度旋转,1:左右翻转,2:不旋转
         self._im = None                                 # 存储当前原始图形的im属性
@@ -3163,16 +3165,15 @@
 
     def _go(self, distance):
         """重定义_go方法,移动指定距离"""
         ende = self._position + self._orient * distance
         self._goto(ende)
         
     def _rotate(self,angle):
-        """seth,right,left最终都要调用它，所以重写它就行了"""
-        
+        """seth,right,left最终都要调用它，所以重写它就行了"""        
         Turtle._rotate(self,angle)         # 调用父类的同名方法
         if self.turtle._type in ['polygon','compound']: return
         if self.shape() == 'blank':return        
                  
         stretch_wid,stretch_len ,w = Turtle.shapesize(self)   # 获取缩放值       
         new_name = self._make_shape_name(str(stretch_wid),str(stretch_len))
         self.shape(new_name)        
@@ -4586,17 +4587,15 @@
             if degrees!=360:
                self.goto(mid)
         self.goto(p1)
         if isfill: self.end_fill()
         self.penup()
         self.goto(old_pos)
         self.setheading(old_heading)
-        return diameter
-        
-        
+        return diameter       
 
     def polar_coordinates(self,reserve=0):  # 返回角色的极坐标
         x,y = self._position
         a = math.degrees(math.atan2(y,x))
         if a<0:a = a  + 360
         a = round(a,reserve)
         p = round((x*x+y*y)**0.5,reserve)
@@ -4703,14 +4702,15 @@
         start = x,y
         screen = self.getscreen()
         tr = screen.tracer()    
         contours,innters = self.find_contours(start,{self.turtle._item}) # 查找轮廓                
         isd = self.isdown()            # 记录当前是否落笔的状态    
         self.penup()                   # 不管当前是否有无落笔,都要抬笔         
         [self.godot(x,y,1,fc) for x,y in contours+innters ]  # 用打点填充内部,速度慢        
+        self.goto(start)               # 回到起始点
         screen.tracer(tr,0)
         if isd:self.pendown()           # 如果填充前是落笔状态,则恢复
         return contours , innters
 
     def fill_convex(self,x,y):        # fill命令模式为0调用的方法 
         """以start为起点,查找封闭图形并进行填充,本函数是测试版本，
            请不要让start在封闭图形外,否则填充时间长导致无响应,并会出现意外!
@@ -4727,45 +4727,50 @@
         isd = self.isdown()            # 记录当前是否落笔的状态    
         self.penup()                   # 不管当前是否有无落笔,都要抬笔
         self.goto(points[0])
         self.begin_fill()         
         [self.godot(x,y,1,fc) for x,y in points[1:] ]        
         self.goto(points[0]) 
         self.end_fill()
-        screen.update()        
+        screen.update()
+        self.goto(start)                # 回到起始点
         screen.tracer(tr,0)
         if isd:self.pendown()           # 如果填充前是落笔状态,则恢复
         return  points,tuple()
         
     def flood_fill(self,x,y): # fill模式为2调用的方法
         """漫水填充方法要调用find_contours,cors2image与fill_area方法"""        
         start = x,y
         screen = self.getscreen()
         tr = screen.tracer()
         screen.tracer(0,0)
         # exds是要排除的item列表,(在用find_contour查找轮廓时要排除一些item
-        pop = self._draw_bubble_turtle
+        pop = self._draw_bubble_turtle        
         exds = screen.fillitems | { self.currentLineItem,self.drawingLineItem,pop.currentLineItem,pop.drawingLineItem}         
+        exds.add(self.turtle._item)                       # 把自己的项目编号加进去 
         contours,innters = self.find_contours(start,exds) # 查找轮廓         
         fc = convert_colorRGBA255(self.fillcolor()) # 把颜色字符串和1.0模式的RGB转为255
         
         fill_area( innters+contours,fc)          # 填充由points组成的最小矩形区域
         fc = self.fillcolor()         # 填充颜色
         
         if isinstance(fc,tuple) and self.screen.colormode()==255:
             fc = int(fc[0]),int(fc[1]),int(fc[2])
         [self.godot(x,y,1,fc) for x,y in contours ]  # 勾勒轮廓
+        self.goto(start)                             # 回到起始点
         screen.tracer(tr,0)
         return contours,innters
           
-    def fill(self,x,y,mode=2):
+    def fill(self,x=None,y=None,mode=2):
         """Sprite类的填充函数，x,y则是封闭图形内的一个点。
            mode:值为0,1,2，值为0时调用凸版，即fill_convex函数，适合于画的图形为凸多边形。
            值为1则调用凹版，即fill_concave函数，适合于任何封装图形，速度较慢，请耐心等待。
            值为3时调用 flood_fill即洪水填充方法，速度还行,注意不要在封闭图形外面填充,会导致无响应。"""            
+        if x==None and y==None:
+            x,y = self.position()
         if mode==0:
             contours,innters = self.fill_convex(x,y)     # 凸
         elif mode==1:           
             contours,innters = self.fill_concave(x,y)    # 凹
         else:           
             contours,innters = self.flood_fill(x,y)      # 洪水填充
         return contours,innters
```

### Comparing `sprites-1.70/sprites.egg-info/PKG-INFO` & `sprites-1.72/sprites.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprites
-Version: 1.70
+Version: 1.72
 Summary: Python Sprites Module for make introductory animations and games and educational purpose。It mainly provides Sprite class inherited from Turtle class。Can be applied to the teaching of elementary mathematics。Pyhton的精灵模块，为教育目的而制作启蒙动画与游戏。主要提供继承自Turtle类的Sprite类,Key类,Mouse类等及一些工具函数,如洪水填充命令,几何相关命令。它支持像素级碰撞检测命令及增强的图章命令等等，也可应用于初等数学几何的教学。作者：李兴球。微信:scratch8，专业编程私教。网址： www.lixingqiu.com
 Home-page: http://www.lixingqiu.com
 Author: lixingqiu
 Author-email: 406273900@qq.com
 License: MIT
 Description: ﻿# Python sprites module introduce
```

