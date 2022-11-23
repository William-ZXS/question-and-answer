
iptables


## 设置失时区

hwclock -r 看看硬件时间
hwclock -s 把系统时间设置为硬件时间

更改时区
rm /etc/localtime
ln -s /usr/share/zoneinfo/Asia/Shanghai /etc/localtime


## 关闭selinux

查看当前selinux的状态
getenforce

临时关闭
setenforce 0

永久关闭，设置后重启生效 或者 setenforce 0
sed -i s#SELINUX=enforcing#SELINUX=disabled# /etc/selinux/config



## free 

