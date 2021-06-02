files里面是debug好的内核源码压缩包，原来的手机镜像img，还有解压和打包镜像的工具。

OpenSourceCode里面是debug好的内核源码。

解包原版boot.img文件，将编译生成的内核文件Image.gz-dtb重命名为kernel，然后替换解包文件夹里的kernel文件，再将文件夹重新打包为boot.img。

(就是原来的zImage-dtb文件,替换解包文件夹里的kernel文件，再将文件夹重新打包为boot.img。)

请注意要及时跟新数据。

实时查看调试信息:cat /proc/kmsg。

adb push被拒绝：请先
adb root
adb remount。

./adb reboot bootloader
./fastboot erase boot
./fastboot flash boot new_boot.img
./fastboot reboot

./mkboot boot.img out
./mkboot out new_boot.img



Powered by Xudong Lu, all right reserved!
