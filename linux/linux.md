
iptables


## 设置失时区

hwclock -r 看看硬件时间
hwclock -s 把系统时间设置为硬件时间

更改时区
rm /etc/localtime
ln -s /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
