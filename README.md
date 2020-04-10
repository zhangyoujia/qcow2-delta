# qcow2-delta

qcow2-delta工具功能列表:
1.	qcow2镜像分配模式转换(convert);
2.	正向增量备份链镜像的正向合并(commit);
3.	正向增量备份链镜像的反向合并(stream);
4.	反向增量备份(与qcow2-bitmap工具共同实现, 使用bitmap/commit功能);
5.	关机状态下克隆镜像(通过nbd设备, 支持跨主机克隆镜像);
6.	开机状态下克隆快照;
7.	支持克隆内存快照, 克隆副本可以直接用来恢复虚拟机到当时的运行状态;

8.	支持IO多簇合并, 优化性能;
9.	支持多协程(IO多深度), 优化性能;
10.	支持全0数据簇ZERO标记设置, 优化性能;
11.	支持write in order(见qemu-img convert功能的write in order), IO顺序保证;
12.	支持断点重试;
13.	支持laio与paio;
14.	支持directio与writeback;
15.	支持IO限速;
16.	支持彩色输出;
17.	支持进度条显示;
18.	支持源镜像基本信息向dmesg输出;
