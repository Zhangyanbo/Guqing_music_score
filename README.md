#古琴谱自动生成程序

##功能

自动从唱名谱中，反推出古琴演奏谱，并能自动判断演奏之方便程度，从而提供一系列演奏谱。

##格式

###按音与散音

`{a, b, c}`：代表第`a`弦，`b`徽`c`分。

例如对于代正调定弦（1,2,4,5,6,1,2），寻找音为4的的演奏谱：

```
In[]:= GetP["4"]

Out[]= {{1, 10, 0}, {1, 5, 6}, {2, 12, 0}, {2, 6, 2}, {3, 0, 0}, {3,
   7, 0}, {4, 7, 6}, {5, 8, 5}, {6, 10, 0}, {6, 5, 6}, {7, 12, 0}, {7,
   6, 2}}
```

得到的数据，例如`{5, 8, 5}`，即：五弦八徽五分

##注

本程序暂时需在Wolfram Mathematica中运行，后面会提供可执行程序。
