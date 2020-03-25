# myStudy
学习记录

## 3.22《计算机是怎样跑起来的》书籍学习记录
### 《计算机是怎样跑起起来的》书籍以计算机三大原则为开端，相继介绍了计算机的结构、手工编程、程序流程、算法、数据结构、面向对象编程、数据库、TCP/IP网络、数据加密、XML、计算机系统以及SE的相关知识。个人觉得是一本新手非常适合阅读的书籍，整体思路清晰明了，有趣的是并不会让人产生枯燥的阅读感受！
### 开端：基础中的基础
#### 1.硬件和软件的区别：硬件（Hardware)代表“硬的东西”而软件（Software)代表“软的东西”。是硬的还是软的取决于眼睛能不能看到，或者实际上是否能够用手触摸到。
#### 2.存储字符串“中国”需要几个字节：存储汉字时，字符编码不同，汉字汉字占用的字节数也就不同，在GBK字符编码下，一个汉字占两个字节。而在UTF-8字符编码下，一个汉字占用3个字节。
#### 3.什么是编码：计算机内部会把所有的信息都当成数字来处理，尽管有些信息本来不是数字。用于表示字符的数字是“字符编码”，用于表示颜色的是“颜色编码”。      
### 第一章核心重点：计算机三大原则
#### 1.计算机是执行输入、运算、输出的机器。
#### 2.程序是指令和数据的集合。
#### 3.计算机的处理方式有时与人们的思维习惯不同。
### 1.2输入、运算、输出是硬件的基础
#### 关键名次：IC。引脚用于输入和输出，IC内部对外部输入的信息进行运算，并且输出到外部。IC（Integrated circnit,集成电路）
#### 1.计算机的由大量的IC组成集成电路。简单的来说，计算机所做的事情就是“输入”数据“1和2”然后对他们执行加法“运算”，最后“输出”计算结果3，输入、运算、输出三者必须成套出现。
### 1.3软件是数据和指令的集合
#### 关键名词：指令，程序。1.指令就是控制计算机进行输入、运算、输出的命令。把向计算机发出的指令一条条列出来就得到了程序。2.程序是指令和数据的集合。
#### 在程序设计中，会为一组指令赋予一个名字，可以称之为“函数”。程序中的数据：1.指令执行对象输入数据 2.指令的执行结果得到输出数据
#### 在编程中时程序员会为数据赋予名字，称其为变量。举例：证明程序是指令和数据的集合，代码清单：C语言的程序实例片段
#### int a,b,c;
#### a=10;
#### b=20;
#### c=Average(a,b),
#### C语言要在每条指令的末尾写一个分号”，第一行“int a,b,c;"表示接下来要使用名为a,b,c的整理变量，其中int是integer(整数）的缩写，用于告诉计算机“要用的是整数”。下一行的“a=10”，表示把整数10赋值给变量a，同样的，“b=20"，表示把整数20赋值给变量b，符号“=”是赋值给变量的指令。再看最后一行的“C=Average(a,b),”，这一行表示把变量a和b传给函数的参数，并把运算结果赋值
#### 给变量C。其中使用一个名为Average的神秘函数，它的作用是返回两个参数的平均值。
#### 无论多么复杂的程序，都不过时=是指令和数据的集合。在一般的编程过程中，都要先编译再执行。所谓编译就是把用C语言编写的文件（源文件）转换为机器语言（原生代码）编写的文件。
### 1.4对计算机来说什么都是数字
#### 使用计算机的母的就是为了提高工作效率。计算机内部先把文字转换为相应的数字叫做“字符编码”，总之计算机会把什么都用数字来表示。
### 1.5只要理解了三大原则，即遍遇到了难懂的最新技术，也能轻松应对。
#### 微软公司率先提出了作为新一代互联网平台NET技术，有关NET的说明：计算机是执行程序的机器。程序是指令和数据的集合。为了使互联网上相互连接的计算机能通过程序协同工作，微软办公室用了SOAP以及XML的规范。SOAP是关于调用指令的规范，XML则是定义数据格式的规范。（只要定义出了指令和数据的规范，装有符合规范的程序计算机就可以相互协作了）
### 1.6为了贴近人类，计算机在不断进化
#### 计算机进化的目的只有一个——与人类更加相近。想要贴近人类，就必须从计算机的处理方式中摒弃不符合人们思维习惯的部分。
#### 具体案例：20世纪80年代个人计算机操作系统是MS——DOS。进入90年代进入Windows（XP代表Exerience 体验）。
#### 编程方式也在进化：面向组件编程（Component Based Prcgramming) 面向对象编程（Object Oriented Prcgramming).面向组件编程的方法是通过将组件（程序零件）组装到一起完成的程序，面向对象的编程的方法是先如实地对现实世界的业务建模，之后再把模型搬到程序中。
## 3.23《计算机是怎样跑起来的》第二章  前三大点学习记录
### 热身问题
#### 1.CPU是什么的缩写：CPU是Central Drocessing Unit（中央处理器）；CPU是计算机的大脑，负责解释，执行程序的内容，有时也将CPU称作处理器
#### 2.HZ是表示什么的单位：HZ（赫兹）是频率的单位。通常用HZ表示驱动CPU运转的信号时钟的频率：一秒发出一次时钟信号就是1HZ，所以100MHZ（兆赫兹）的话就是100✖️100万=一亿次/秒.M（兆）代表百万
#### 3.Z80 CPU是多少比特的CPU：Z80是8比特的CPU。CPU上数据总线的条数，或者CPU内部参与运算的寄存器的数量，都可以作为衡量CPU性能的比特数。在Z80 CPU中，无论是数据的条数还是寄存器的容量都是8比特，所以Z80 CPU是一款8比特的CPU。而在Windows个人计算机中广泛应应用的Pentium(奔腾）CPU则是32比特CPU。
### 2.1制作微型计算机所必需要的元件
#### 1.CPU：CPU是计算机的大脑，负责解释执行程序。
#### 2.内存：负责存储程序和数据。
#### 3.1/O是INput/Qutuput(输入和输出）的缩写，负责将计算机和外部设备（周边设备）连接在一起。
### 关键名词：元件型号（CPU——Z80 TC5517——内存 Z80 PIO作为I/O）
### 关键名词解释
#### Z80 CPU是一款古老的CPU，在NEC的PC—8801，SHARP的M2—80等比特广泛应用的时代，曾以爆炸般的速度普及过。
#### TC5517是可以存储2k的8比特数据的内存。解释：k表示2的十次方=1024。TC5517的容量是8比特✖️2✖️1024=16384比特，即2k字节。
#### PIO（Parullel I/O，并行输入/输出）可以在微型计算机和外部设备之间并行地（一排一排地）输入输出8比特的数据。
#### “时钟信号"：电信号好比一个时钟，每间隔一次时间就变换一次电压的高低。输出时钟信号的元件叫做“时钟发生器”，发生器中带有晶振，根据自生频率产生时信号。时钟信号可以可以衡量CPU的运转速度。
#### 指波开关是一种由8个开关并排连在一起构成的元件，在这里通过拨动开关来输入程序。
#### 电阻是用于阻碍电流流动，降低电压值的元件，单位欧姆。
#### 电容是存储电荷的元件，衡量在储电荷能力的单位是法拉。
### 2.2电路图的读法
#### 关于电路图的读法：在电路图中有些地方有交叉，但若只是交叉在一起的话，并不表示在交叉处构成通路。只有在交叉点外再画上一个小黑点才表示构成通路。
### 2.3连接电源数据和地址总线
#### 280 CPU、TC5517和280 PIO上都分别带有VCC引脚和GND引脚（VCC引脚和GND这一对引脚用于为IC供电）
#### 连线方式：先将+5V电源连接到各个IC的VCC引脚上，然后0V电源连接到各个IC的GND引脚上，接下来还需要将+5V和0V连接到时钟发生器上，最后接通电源。
#### 原理：微型计算机所使用的IC属于数字IC。在数字IC中，每个引脚上的电压要么是0V，要么是+5V，通过这两个电压，与其他的IC进行电信号的收发。用于给IC供电的VCC和GND的引脚上的电压是恒定不变的+5V和0V，但是其他引脚上的电压，会随着计算机的操作在+5V和0V之间不断的变化。
#### 关于二进制的知识点：通常将一个二进制数也就是数字IC上一个引脚所能表示的0或者1，所表示的信息称作“1特比”将8个二进制数（也就是8比特）称作“字节”比特是信息最小的单位，字节是信息最基本的单位。
#### 计算机以CPU。为中心的连接方式：CPU可以与内存或I/O进行数据的输入和输出。为了指定输入输出数据的源头和目的为了指定输入输出数据时的源头或目的地，CPU上备有“地址总线引脚”。Z80 CPU的地址总线引脚共有16个，用代号A0～A15表示，其中的A表示Address（地址）。后面的数字0～15表示一个16位的二进制数中各个数字的位置，0对应最后一位、15对应第一位。16个地址总线引脚所能指定的地址共有65536个，用二进制数表示的话就是0000000000000000～1111111111111111。因此Z80 CPU可以指定65536个数据存取单元（内存存储单元或I/O地址），进行信息的输入输出。一旦指定了存取数据的地址，就可以使用数据总线引脚进行数据的输入输出了。Z80 CPU的数据总线引脚共有8个，用代号D0～D7表示。其中的D表示Data（数据），后面的数字0～7与地址总线引脚代号的规则相同，也表示二进制数中各个数字的位置。Z80 CPU可以一次性地输入输出8比特的数据，这就意味着如果想要输入输出位数（比特数）大于8比特的数据，就要以8比特为单位切分这个数据。作为内存的TC5517上也有地址总线引脚（A0～A10）和数据总线引脚（D0～D7）。这些引脚需要同Z80 CPU上带有相同代号的引脚相连。一块TC5517上可以存储2048个8比特的数据（如图2.6所示）。可是由于用于输入程序的指拨开关是以8比特为一个单位指定内存地址的，所以我们只使用TC5517上的A0～A7这8个引脚，并把剩余的A8～A10引脚连接到0V上（这些引脚上的值永远是0）。
## 3.24号:yum:关于掌握Warkdown语法和写作格式的学习 《计算机是怎样跑起来的》2.5章节到2.7章节的学习
### 掌握Markdown
#### Mastering是一种在网页上设置文本样式的方法。你控制文档的显示；格式化单词为粗体或斜，添加图像和创建列表，这些只Markdownk可以胜任的一部分工作而已。在通常情况下，Markdown只是引入了一些非字母字符（例如#或*）的常规文本。
### :yum:具体的学习记录以文字书写记录，我将在在接下来的文本练习中反复尝试建立更加有趣的学习记录:yum:
### 2.5连接时钟信号
#### 为了传输时钟信号，就需要把时钟发生器的8号引脚和Z80 CPU的CLK（CLK即Clock，时钟）引脚Z80 PIO的CLK引脚分别连起来。
### 2.6连接用于区分读写对象是内存还是1/O的引脚
#### 名词解释
#### MAEQ（即Memory Request,内存请求）
#### IORQ（即I/O Request,I/O请求
#### CE（即Chip enable,连通芯片）
#### 原理：当Z80 CPU和内存之间有数据输入输出时，MREO引脚上的值是0，反之则是1。当Z80 CPU和I/O之间有数据输出时，IORQ引脚上的值是0反正则是1。
### 2.7连接剩余的控制引脚
#### 名词解释
#### 控制引脚：CPU内存，I/O中不但有地址总线引脚，数据总线引脚，通常把这些引脚统称为为控制引脚。
#### MI引脚（即Miachine Cycle 1 机器周期1）：是用于同步的引脚。
#### INT引脚（即Interrupt,中断）：是用于从Z80 PIO向Z80 CPU发出中断请求的引脚（让CPU根据外部输入的数据执行待定的程序）。
#### RESET引脚（即Reset,重置）
#### BUSRQ引脚（即Bus Request,总线请求）
#### DMA（Direct Menory Access)，直接存储器访问）：不经过CPU直接从外部设备续写内存的行为。
#### 上拉（Puu-UP)
#### 关于计算机工作原理：CPU在时钟信号的控制下解释、执行内存中存储的程序。按照程序中的指令从内存或I/O中把数据输入到CPU中，在CPU内部进行运算，再把运算结果输入到内存或I/O中。
## 3.25:yum:《计算机是怎样跑起来的》2.8章到2.10章学习
### 2.8连接外部设备，通过DMA输入程序
#### 原理：使用两个指拨开关和一个按键开关向地方总线引脚和数据总线引脚发送电信号，然后通过DMA将数据总线上的数据存储到内存。
### 2.9连接用于输入输出的外部设备
#### 74367是一种叫做“三态总线缓冲器”的IC
#### 当微形计算机运行起来后，指拨开关可用于从外部输入设备数据，LED可用于向外部输出数据。
### 2.10输入测试程序并进行调试
#### 作为计算机大脑的CPU能解释执行一种编程语言，那就是靠罗列二进制数构成的机器语言（原生代码）。
