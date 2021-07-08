---
title: "使用移位运算符"
date: "2018-05-26 17:31:46"
tags: ["算法"]
categories: ["算法"]
---
```
middle = (L+R)/2
这样的写法 L+R 有可能溢出
```

```
  middle = L + (R-L)/2
=>minddle = L + (R-L)>>1 
```

这样写的好处是不会发生数据溢出，除以 2 则是向右移一位，位运算比算术运算快