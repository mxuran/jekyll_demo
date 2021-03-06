---
layout: default
title: git与github的连接和使用(linux版)
---
## git与github的连接和使用(linux版)

[^]: 教程为deepin操作系统,debian系列都可使用(如:ubuntu)

#### 一 git的安装

------



1. 安装git

   ```
   sudo apt-get install git
   ```

   ![](https://github.com/mxuran/image/raw/master/2019-2-2-CSDN/1549024129647.png)

2. git配置

   ```
   git config --global user.name "这里改为你的名字"
   git config --global user.email "这里改为你的邮箱地址"
   ```

   ![](https://github.com/mxuran/image/raw/master/2019-2-2-CSDN/1549024511043.png)

3. 创建公钥

   ```
   ssh-keygen -C '这里改为你的邮箱地址' -t rsa
   ```

   [^注]: 输入命令后一路回车,如果提示输入y/n,输入y即可.

   ![](https://github.com/mxuran/image/raw/master/2019-2-2-CSDN/1549025061570.png)

4. 复制公钥内容

   - 进入~/.ssh文件夹

   ```
   cd ~/.ssh
   ```

   - 打开id_rsa.pub文件(deepin编辑器为dedit命令,ubuntu为gedit),复制内容.(此处若无法打开,则找到文件,用wps即可打开)

   ```
   dedit id_rsa.pub
   ```

   ![](https://github.com/mxuran/image/raw/master/2019-2-2-CSDN/1549025709050.png)





#### 二 github的连接

1. 配置公钥

   ![](https://github.com/mxuran/image/raw/master/2019-2-2-CSDN/1549027054007.png)

2. 新建一个仓库

   ![](https://github.com/mxuran/image/raw/master/2019-2-2-CSDN/1549026307329.png)

3. 输入Repository name后,点击Create repository

   ![](https://github.com/mxuran/image/raw/master/2019-2-2-CSDN/1549026364296.png)

4. 在本地创建名为example的repository

   ```
   git init example
   cd example
   ```

   ![](https://github.com/mxuran/image/raw/master/2019-2-2-CSDN/1549027648228.png)

5. 编写README文件

   ```
   dedit README
   ```

   ![](https://github.com/mxuran/image/raw/master/2019-2-2-CSDN/1549028982530.png)

6. 依次执行以下命令

   ```
   git add README
   git commit -m "这里改为你自己想注释的内容"
   git remote add origin https://github.com/这里改为你自己的github名字/example.git
   git push origin master
   ```

   ![](https://github.com/mxuran/image/raw/master/2019-2-2-CSDN/1549029159099.png)

7. 大功告成!![](https://github.com/mxuran/image/raw/master/2019-2-2-CSDN/1549029481647.png)

