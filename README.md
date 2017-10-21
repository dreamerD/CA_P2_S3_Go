# CA_P2_S3_Go
32位MIPS五级流水线处理器第三阶段设计——(乘除法器，MULT...MFHI...BGEZ...JALR)

本阶段所需修改：
1. 添加15条指令，分别为DIV、DIVU、MULT、MULTU、MFHI、MFLO、MTHI、MTLO、BGEZ、BGTZ、BLEZ、BLTZ、BLTZAL、BGEZAL、JALR
具体为：(1)在Control Unit中添加上述指令的控制逻辑；
       (2)添加HI、LO寄存器及其数据通路；
       (3)编写乘除法器，切分为/*2*/级流水，将其嵌入数据通路中。乘法器采用booth算法+华莱士树，除法采用迭代算法。
       (4)...
