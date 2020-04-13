# Github.io博客的搭建

##### 1. github的repositories的新建

![image-20200413163317701](C:\Users\timesong\AppData\Roaming\Typora\typora-user-images\image-20200413163317701.png)

##### 2. 对这个repositories进行Settings进行配置，主要是进行主题选择

![image-20200413163509684](C:\Users\timesong\AppData\Roaming\Typora\typora-user-images\image-20200413163509684.png)

##### 3.在http://jekyllthemes.org/下载一个主题

![image-20200413163732330](C:\Users\timesong\AppData\Roaming\Typora\typora-user-images\image-20200413163732330.png)

##### 4.将github中的repositories进行clone到本地某个文件夹，然后将上述下载的主题放入到该文件夹中，并替换config.yml和README文件夹

1.   先新建一个文件夹存放本地资源，在该文件夹右键打开git bash命令，使用git命令将repositories克隆到本地  **git clone https://github.com/CKTim/BlueTooth.git（https://github.com/CKTim/BlueTooth.git替换成你之前复制的地址）**

2. 将下载的主题放入到该文件夹下，并对新的对config.yml进行替换，除了一些基本信息外，主要修改如下

   ![image-20200413165101846](C:\Users\timesong\AppData\Roaming\Typora\typora-user-images\image-20200413165101846.png)

   | 名称         | 存放文件夹 |
   | ------------ | ---------- |
   | 关于         | about      |
   | 归档         | archive    |
   | 标签         | tags       |
   | 首页存放地址 | _posts     |

3.将本地仓库上传到远程仓库

| **git add .     （注：别忘记后面的.，此操作是把Test文件夹下面的文件都添加进来）** |
| ------------------------------------------------------------ |
| **git commit  -m  ”提交信息”  （注：“提交信息”里面换成你需要，如“first commit”）** |
| **git push -u origin master  （注：此操作目的是把本地仓库push到github上面，此步骤需要你输入帐号和密码）** |

**如果不是第一次上传，则需要在最开始之前进行pull操作**

**git pull --rebase origin master**

