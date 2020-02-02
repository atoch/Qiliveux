# Qilivux
Lubuntu installation on cheap Qilive Q9 windows 10 tablet

Q9 tablet specs:
https://www.auchan.fr/qilive-tablette-tactile-avec-clavier-10-1-w10-866311-noire-32go/p-c915897
Not too bad for 80 Euro (discounted price for a returned unit).

**lspci**
00:00.0 Host bridge: Intel Corporation Atom/Celeron/Pentium Processor x5-E8000/J3xxx/N3xxx Series SoC Transaction Register (rev 36)
00:02.0 VGA compatible controller: Intel Corporation Atom/Celeron/Pentium Processor x5-E8000/J3xxx/N3xxx Integrated Graphics Controller (rev 36)
00:03.0 Multimedia controller: Intel Corporation Atom/Celeron/Pentium Processor x5-E8000/J3xxx/N3xxx Series Imaging Unit (rev 36)
00:0b.0 Signal processing controller: Intel Corporation Atom/Celeron/Pentium Processor x5-E8000/J3xxx/N3xxx Series Power Management Controller (rev 36)
00:14.0 USB controller: Intel Corporation Atom/Celeron/Pentium Processor x5-E8000/J3xxx/N3xxx Series USB xHCI Controller (rev 36)
00:1a.0 Encryption controller: Intel Corporation Atom/Celeron/Pentium Processor x5-E8000/J3xxx/N3xxx Series Trusted Execution Engine (rev 36)
00:1f.0 ISA bridge: Intel Corporation Atom/Celeron/Pentium Processor x5-E8000/J3xxx/N3xxx Series PCU (rev 36)

**lsusb**
Bus 002 Device 001: ID 1d6b:0003 Linux Foundation 3.0 root hub
Bus 001 Device 012: ID 0bda:574c Realtek Semiconductor Corp. USB 2.0 Hub
Bus 001 Device 011: ID 2149:2715 Advanced Silicon S.A. 
Bus 001 Device 010: ID 045e:07b2 Microsoft Corp. 2.4GHz Transceiver v8.0 used by mouse Wireless Desktop 900
Bus 001 Device 009: ID 05e3:0610 Genesys Logic, Inc. 4-port hub
Bus 001 Device 008: ID 152d:0567 JMicron Technology Corp. / JMicron USA Technology Corp. JMS567 SATA 6Gb/s bridge
Bus 001 Device 007: ID 2109:2812 VIA Labs, Inc. VL812 Hub
Bus 001 Device 006: ID 17e9:4306 DisplayLink 
Bus 001 Device 005: ID 17e9:4306 DisplayLink 
Bus 001 Device 004: ID 2109:2812 VIA Labs, Inc. VL812 Hub
Bus 001 Device 003: ID 258a:000c  
Bus 001 Device 002: ID 1a40:0801 Terminus Technology Inc. USB 2.0 Hub
Bus 001 Device 001: ID 1d6b:0002 Linux Foundation 2.0 root hub

**lsusb**
Bus 002 Device 001: ID 1d6b:0003 Linux Foundation 3.0 root hub
Bus 001 Device 012: ID 0bda:574c Realtek Semiconductor Corp. USB 2.0 Hub
Bus 001 Device 011: ID 2149:2715 Advanced Silicon S.A. 
Bus 001 Device 010: ID 045e:07b2 Microsoft Corp. 2.4GHz Transceiver v8.0 used by mouse Wireless Desktop 900
Bus 001 Device 009: ID 05e3:0610 Genesys Logic, Inc. 4-port hub
Bus 001 Device 008: ID 152d:0567 JMicron Technology Corp. / JMicron USA Technology Corp. JMS567 SATA 6Gb/s bridge
Bus 001 Device 007: ID 2109:2812 VIA Labs, Inc. VL812 Hub
Bus 001 Device 006: ID 17e9:4306 DisplayLink 
Bus 001 Device 005: ID 17e9:4306 DisplayLink 
Bus 001 Device 004: ID 2109:2812 VIA Labs, Inc. VL812 Hub
Bus 001 Device 003: ID 258a:000c  
Bus 001 Device 002: ID 1a40:0801 Terminus Technology Inc. USB 2.0 Hub
Bus 001 Device 001: ID 1d6b:0002 Linux Foundation 2.0 root hub

**df**
Filesystem      1K-blocks       Used  Available Use% Mounted on
udev               936416          0     936416   0% /dev                                                                                                                 
tmpfs              196292       2028     194264   2% /run                                                                                                                 
/dev/mmcblk0p3   28468320    7314348   19684788  28% /                                                                                                                    
tmpfs              981444     176832     804612  19% /dev/shm                                                                                                             
tmpfs                5120          4       5116   1% /run/lock                                                                                                            
tmpfs              981444          0     981444   0% /sys/fs/cgroup                                                                                                       
/dev/loop0          91264      91264          0 100% /snap/core/8268                                                                                                      
/dev/loop1         185472     185472          0 100% /snap/spotify/36                                                                                                     
tmpfs              196288          8     196280   1% /run/user/1000                                                                                                       
/dev/sdb1      5860520896 4016925888 1843595008  69% /media/arnaud/Data_NTFS                                                                                              
/dev/sda2      5860389824 3997452800 1862937024  69% /media/arnaud/Data2                                                                                                  
/dev/sdd3       502914096    1125996  476171716   1% /kernel     

Installation was impossible from the iso burned on the USB key until the tablet was connected to external HDMI monitor. Lubuntu as other distributions I tried would get me only a grey screen probably due to the 800x1200 native resolution of the tablet's screen.

Installation
Package management
Displaylink
Sound
Tablet screen
Kernel:https://github.com/atoch/Qiliveux/blob/master/Kernel.md
Netflix
SDCard
Power Management
