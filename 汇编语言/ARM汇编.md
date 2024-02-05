# ARM汇编
## 1.介绍
1. ARM指令只处理寄存器中的数据，不需要缓存操作，操作速度很快
2. 与Intel CPU相比，ARM CPU实现1个功能，需要更多的指令，但指令执行
时间短。
3. ARM具有两种运行模式/工作状态，32位ARM模式和16位Thumb模式
4. Intel架构指令集是CISC，ARM架构指令集是RISC，ARM架构与Intel架构比
较，RAM CPU中有更多的寄存器。   

## 编译平台
1. ARM公司的汇编器，集成到了各种嵌入式开发的IDE中，适用于Windows系统：ADS1.2，KeiluVision等。
2. GNU交叉编译工具链中的汇编器，适用于Linux系统中gnu arm汇编，程序风格更个接近于AT&T风格，编译器是arm-linux-gcc。
