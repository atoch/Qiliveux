**Kernel**

Kernel has to be compiled to allow building DisplayLink driver for Ubuntu 20.04
Lubuntu comes with stock Ubuntu kernel (all Ubuntu variantes do): 5.4.0

Kernel source contains a lot of files. It is preferable to use an external USB 3 hard drive to avoid filling the internal mmc. As compilation generate object files, for the mmc longevity, it is also better to compile and build the kernel on a fast magnetic disk.

```make -j 4 # to compile using 4 threads on this 4 cpus tablet

sudo make modules_install -j 12  

sudo make install -j 12  

sudo update-grub
``` 

To do: 
- kernel optimization
- kernel update
