penwrt-study
=============
最近在使用百度联想新路由mini，刷的是基于openwrt的pandorabox，发现shell下有好多命令都木有，比如nohup、unrar等命令，所以交叉编译了下放到git里共享下。

使用的交叉编译工具链是：http://downloads.openwrt.org/barrier_breaker/14.07/ramips/mt7620a/OpenWrt-Toolchain-ramips-for-mipsel_24kec%2bdsp-gcc-4.8-linaro_uClibc-0.9.33.2.tar.bz2
仅适用于相同的架构：小米路由mini也是使用的相同架构，所以也是可以用这个toolchain编译的

git中的每个文件夹对应一个命令，再向下的bin目录放着编译好的二进制文件，下载直接就可以用了，src目录放着源码，可自行编译

备注：其实我就是想用路由器下几部片片，没有nohup不好用，不知道为什么默认的opkg库中没有这个工具包，另外有些种子下载下来的文件竟然是rar格式的，泪奔……只好再弄个unrar工具了。
