# Embed-sumer-eri
嵌入式QEMU、BUILDROOT、ZCU102安装步骤

写在前面：

 Qemu：一种虚拟机，用于模拟计算机硬件环境。
 Buildroot：整个Buildroot是由Makefile脚本和Kconfig配置文件构成的。你可以和编译Linux内核一样，通过buildroot配置，menuconfig修改，编译出一个完整的可以直接烧写到机器上运行的Linux系统软件(包含boot、kernel、rootfs以及rootfs中的各种库和应用程序)。


1.下载
Buildroot：https://buildroot.org/downloads/buildroot-2019.02.3.tar.gz
Qemu xlnx：https://github.com/Xilinx/qemu
ZCU102：

2.安装
（1）Buildroot的安装：
 tar -zxvf buildroot-2019.02.3  #解压buildroot
 cd buildroot-2019.02.3         #打开buildroot解压后文件夹    
 make menuconfig                #打开配置页面，进行自定义配置
 make                           #根据自定义配置进行编译
 
 （2）Qemu的安装：
 安装步骤：https://xilinx-wiki.atlassian.net/wiki/spaces/A/pages/18842060/QEMU
 （3）zcu102配置：
 只需将zcu102文件夹所在位置进行正确配置即可使用。
 
 
 
 


