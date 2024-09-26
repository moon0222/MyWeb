# 计算机图形学

#### Rasterization or Scan conversion 栅格化

###### CRT (电子管显示器)

###### LCD (液晶显示器)

由液晶控制偏振方向控制光的强弱

显示黑色存在漏光现象

###### LED

##### Raster Graphic Packages

a collection of efficient algorithms

> Coordinate System

将像素定义在整数格点上

Given a line segment defined by its endpoints, determine the pixels and color which best model the line segment

y = mx + c  rounding

###### Digital Differential Analyzer (DDA)

x~i~ = x~i-1~ +1

y~i~ =  y~i-1~ +m

[x~i~ , round(y~i~)]

###### Bresenham's Line Drawingh 

y = m(x~i~ +1)+b

d~1~ = y - y~i~

d~2~ = y~i~ +1 - y

if d~1~ -d~2~ >0, then y~i+1~ = y~i~ + 1, else y~i+1~ = y~i~

```
plot(x_1,y_1); dx = x2-x1, dy = y2-y1, P1 = 2dy-dx
x_i+1 =x_i +1
if Pi > 0, then y_i+1 = y_i + 1; else y_i+1 = y_i
```

```
dx = x2 - x1
dy = y2 - y1
m = dy/dx

xi = x1
yi = y1
pi = 2dy - dx

while xi != x2 + 1
    if Pi < 0
        pi = pi + 2dy
        yi = yi
    else
        pi = pi + 2dy - 2dx
        yi = yi + 1
#将下一个像素(x,y)涂色
    plot(xi, yi)
    xi = xi + 1
```

画圆 -- 极坐标

画多边形 -- Winding number

Scan-line method

Seed Fill Algorithm

##### Clipping (裁剪)


### OpenGL

GLU, GLUT, GLUI 



OpenGL is a state machine

* All ( command names/ Data types )begin with gl: glVertex3f

Colors -RGB








