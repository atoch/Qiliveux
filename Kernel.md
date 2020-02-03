**Kernel**

Kernel has to be compiled to allow building DisplayLink driver for Ubuntu 20.04
Lubuntu comes with stock Ubuntu kernel (all Ubuntu variantes do): 5.4.0

`uname -a`
> Linux qilivux 5.4.0-12-generic #15-Ubuntu SMP Tue Jan 21 15:12:29 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux



Kernel source contains a lot of files. It is preferable to use an external USB 3 hard drive to avoid filling the internal mmc. As compilation generate object files, for the mmc longevity, it is also better to compile and build the kernel on a fast magnetic disk.

```
make -j 4 # to compile using 4 threads on this 4 cpus tablet

sudo make modules_install -j 4

sudo make install -j 4

sudo update-grub
``` 

After the update-grub
> arnaud@qilivux:/proc$ ls -l /boot

> total 114940

> -rw-r--r-- 1 root root   237699 janv. 21 14:43 config-5.4.0-12-generic

> -rw-r--r-- 1 root root   237688 févr.  3 20:00 **config-5.4.8**

> drwx------ 3 root root     4096 janv.  1  1970 efi

> drwxr-xr-x 5 root root     4096 févr.  1 19:01 grub

> lrwxrwxrwx 1 root root       27 janv. 31 17:44 initrd.img -> initrd.img-5.4.0-12-generic

> -rw------- 1 root root 84075203 févr.  2 18:54 initrd.img-5.4.0-12-generic

> lrwxrwxrwx 1 root root       27 janv. 31 17:44 initrd.img.old -> initrd.img-5.4.0-12-generic

> -rw-r--r-- 1 root root   182704 janv. 28  2016 memtest86+.bin

> -rw-r--r-- 1 root root   184380 janv. 28  2016 memtest86+.elf

> -rw-r--r-- 1 root root   184840 janv. 28  2016 memtest86+_multiboot.bin

> -rw------- 1 root root  4712577 janv. 21 14:43 System.map-5.4.0-12-generic

> -rw-r--r-- 1 root root  4683920 févr.  3 20:00 System.map-5.4.8

> lrwxrwxrwx 1 root root       13 févr.  3 20:00 **vmlinuz -> vmlinuz-5.4.8**

> -r--r--r-- 1 root root 11584248 févr.  1 18:59 vmlinuz-5.4.0-12-generic

> -rw-r--r-- 1 root root 11578240 févr.  3 20:00 vmlinuz-5.4.8

> lrwxrwxrwx 1 root root       24 janv. 31 17:44 vmlinuz.old -> vmlinuz-5.4.0-12-generic



To do: 
- kernel optimization
- kernel update
