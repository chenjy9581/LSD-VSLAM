### LSD-VSLAM
经过修改完善Ubuntu 16.04+ROS-kinetic下可直接编译的LSD算法包.

安装过程如下：
```
# 创建工作空间
$ mkdir -p ~/catkin_lsd/src
# 安装依赖
$ sudo apt-get install ros-kinetic-libg2o ros-kinetic-cv-bridge liblapack-dev libblas-dev freeglut3-dev libsuitesparse-dev libx11-dev
$ sudo apt install libqglviewer-dev-qt4
#修改配置
$ cd /usr/lib/x86_64-linux-gnusudo 
$ ln -s libQGLViewer-qt4.so libQGLViewer.so
#编译
$ cd  ~/catkin_lsd
$ catkin_make
```