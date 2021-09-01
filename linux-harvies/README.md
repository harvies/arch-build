
## 图形化配置内核
make menuconfig

## 编译内核 跳过签名验证
makepkg -s --skippgpcheck --skipchecksums

## 安装内核及头文件
sudo pacman -U linux-harvies-*

## 更新引导
grub 
sudo grub-mkconfig -o /boot/grub/grub.cfg

systemd-boot
配置启动项
vim /boot/loader/entries/xxx.conf
