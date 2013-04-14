# rpi-rtl8188eu

Linux driver for tplink-wn725n nano wireless adapter.

The source code is from https://github.com/Red54/linux-shumeipai2/tree/sunxi-3.0/drivers/net/wireless/rtl8188eu and updated from the patch https://bugs.launchpad.net/ubuntu/+source/linux/+bug/1030858/+attachment/3465019/+files/use_kthread_run.patch

## compile and install

1. make
2. copy 8188eu.ko to ``/lib/modules/`uname -r`/kernel/driver/net/wireless``
3. depmod -a
4. modprobe 8188eu
5. ifconfig and you can see the wlan interface :-)