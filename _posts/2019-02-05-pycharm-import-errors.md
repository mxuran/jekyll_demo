---
layout: default
title: pycharm导入同一个包下的py文件错误
---
## pycharm导入同一个包下的py文件错误

1. 问题描述

   相同的`python pakage`下,在一个`py`文件中`import`另一个`py`文件,显示错误,如下图红线.

   ![1549374707634](https://github.com/mxuran/image/raw/master/2019-2-5-CSDN/1549374707634.png)

2. 解决方案

   鼠标右键`python package`, 选择`Mark  Directory as`, 然后点击`sources root`.

   ![1549374902178](https://github.com/mxuran/image/raw/master/2019-2-5-CSDN/1549374902178.png)

3. 此时已经没有红色错误, 效果如下.

   ![1549375032251](https://github.com/mxuran/image/raw/master/2019-2-5-CSDN/1549375032251.png)

   