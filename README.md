# 个人博客地址：www.wanuse.com


下载源代码，更新 feeds 并选择配置

git clone https://github.com/openwrt/openwrt \
cd openwrt \
./scripts/feeds update -a \
./scripts/feeds install -a \
make menuconfig \
下载 dl 库，编译固件 （-j 后面是线程数，第一次编译推荐用单线程） \
make download -j8 \
make V=s -j1
