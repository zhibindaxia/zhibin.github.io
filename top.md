#top

```powershell
top - 11:51:51 up  3:41,  1 user,  load average: 2.77, 1.50, 1.20
任务: 330 total,   1 running, 261 sleeping,   0 stopped,   0 zombie
%Cpu(s):  7.8 us,  1.5 sy,  0.0 ni, 90.7 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st
KiB Mem :  8092424 total,   326344 free,  4214064 used,  3552016 buff/cache
KiB Swap:  8311804 total,  8311804 free,        0 used.  2260628 avail Mem 

进程 USER      PR  NI    VIRT    RES    SHR �  %CPU %MEM     TIME+ COMMAND     
 2175 peng      20   0 9796648 490472 218988 S  39.9  6.1  91:30.36 chrome      
 1608 peng      20   0 4445172 253360 141792 S  10.6  3.1  16:51.49 gnome-shell 
 2125 peng      20   0  788808 277864 211456 S   6.0  3.4  34:08.88 chrome      
 1437 peng      20   0  647456 102388  80420 S   5.6  1.3  15:32.99 Xorg  
```

01:06:48    当前时间   系统运行时间，格式为时:分
1 user    当前登录用户数
load average : 1.06, 1.07, 1.08    系统负载，即任务队列的平均长度。三个数值分别为 1分钟、5分钟、15分钟前到现在的平均值。

第二、三行为进程和CPU的信息。当有多个CPU时，这些内容可能会超过两行。内容如下：
total 进程总数
running 正在运行的进程数
sleeping 睡眠的进程数
stopped 停止的进程数
zombie 僵尸进程数
Cpu(s): 
0.3% us 用户空间占用CPU百分比
1.0% sy 内核空间占用CPU百分比
0.0% ni 用户进程空间内改变过优先级的进程占用CPU百分比
98.7% id 空闲CPU百分比
0.0% wa 等待输入输出的CPU时间百分比
0.0%hi：硬件CPU中断占用百分比
0.0%si：软中断占用百分比
0.0%st：虚拟机占用百分比

Mem:
191272k total    物理内存总量
173656k used    使用的物理内存总量
17616k free    空闲内存总量
22052k buffers    用作内核缓存的内存量
Swap: 
192772k total    交换区总量
0k used    使用的交换区总量
192772k free    空闲交换区总量
123988k cached    缓冲的交换区总量,内存中的内容被换出到交换区，而后又被换入到内存，但使用过的交换区尚未被覆盖，该数值即为这些内容已存在于内存中的交换区的大小,相应的内存再次被换出时可不必再对交换区写入
