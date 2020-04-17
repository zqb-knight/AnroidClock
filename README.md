# AnroidClock
## How to use

- Relesse下载app-debug.apk

- 对应目录下终端运行

  **adb install -t app-debug.apk**

## TO-DO 1: 每一秒刷新一次，让指针动起来

本质上是使用handler实现

```java
postInvalidateDelayed(1000);
```



## TO-DO 2: 画分针

```java
drawPointer(canvas,1,nowMinutes);
```



## TO-DO 3: 画分针，设置分针的颜色

```java
degree = value * UNIT_DEGREE;
                mNeedlePaint.setColor(Color.BLUE);
                pointerHeadXY = getPointerHeadXY(MINUTE_POINTER_LENGTH, degree);
```



Updated on 2020-4-17