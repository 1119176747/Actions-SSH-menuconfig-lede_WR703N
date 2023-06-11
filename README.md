# Actions-SSH-menuconfig
功能：使用Actions配置编译openwrt所需的配置文件.config
进入SSH
cd /home/runner/lede
make menuconfig 全局配置
上传供下载
默认是会上传.config的文件的
如果配置多个需要
mkdir zzzzz  #创建目录
cp .config /home/runner/lede/zzzzz/.config1  #复制文件
选用插件
luci-app-arpbind #IP/MAC绑定
luci-app-autoreboot #支持计划重启
passwall或者RRS-plus
固件采用https://github.com/coolsnowwolf/lede的
版本采用了一个修改分支，我编译时好像就这个分支可以用

参考
https://github.com/P3TERX/Actions-OpenWrt
https://github.com/blueveryday/lede_WR703Nv1
https://github.com/songchenwen/openwrt-package
