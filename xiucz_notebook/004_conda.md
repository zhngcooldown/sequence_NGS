##
```python## 设置channel，用于让conda寻找软件所在位置conda config --add channels conda-forgeconda config --add channels defaultsconda config --add channels rconda config --add channels bioconda## 已经添加的channelsconda config --get channels## 更新condaconda update conda## conda默认安装软件的最新版本，如果想安装指定版本的某个软件，可以先搜索软件版本conda search 软件名## 星号标记的表示是已经安装的版本。要安装其他版本，输入：conda install 软件名=版本号## 再次查看已安装软件列表conda list```## 添加镜像源```conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/conda config --set show_channel_urls yesconda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/msys2/```## 推荐新建工作环境下安装软件;```pythonconda create -n aligners bwa bowtie hisat star -y# create -n aligner:新建一个名为alinger的工作环境# bwa bowite hista star： 同时安装这三个软件# -y yes：和Linux的选项一样```## 利用源码压缩文件安装```python## 从https://anaconda.org/bioconda 频道中下载压缩包## 然后把这些解压缩文件全部拷贝到conda下cp -r * ~/miniconda2/## 虚拟环境cp -r * ~/miniconda2/envs/biostar/```
## BioContainer
## Reference_Infohttp://mp.weixin.qq.com/s/nK1Kkf9lfZStoX25Y7SzHQ  https://zhuanlan.zhihu.com/p/25085567  http://www.biotrainee.com/thread-1901-1-1.html  什么是虚拟环境：http://blog.csdn.net/pipisorry/article/details/39998317  https://mp.weixin.qq.com/s/1HOQ8J2vs-lEwdVAxeNiyQ