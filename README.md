# CA_P2_S3_Go
32位MIPS五级流水线处理器第三阶段设计——(乘除法器，MULT...MFHI...BGEZ...JALR)

### 本阶段所需修改：

添加15条指令，分别为DIV、DIVU、MULT、MULTU、MFHI、MFLO、MTHI、MTLO、BGEZ、BGTZ、BLEZ、BLTZ、BLTZAL、BGEZAL、JALR

具体为：

* 在Control Unit中添加上述指令的控制逻辑
* 添加HI、LO寄存器及其数据通路
* 编写乘除法器，切分为X(e.g.,2)级流水，将其嵌入数据通路中。乘法器采用booth算法+华莱士树，除法采用迭代算法
* BGE、BGT、BLT、BLE可以用rs[31]和rs[30:0]的值来判断。比如BGTZ指令中，若rs[31]=0 & rs[30:0]!=0，则执行跳转。这可以通过添加一个统一的译码模块并给出控制信号来实现
* ...
