# CN-Lab-Go-back-N-protocol
BIT 2023 Spring Computer Network Programming Project 1

本项目为BIT20级计算机网络第一次编程作业。实现了在电脑上通过两个终端分别运行host.exe完成全双工通信。当然，因为时间问题还有一些细节没有完善，比如传输的文件的类型多元化等等。

## 项目构成

*LogAnalyzer.py*：用于读取日志文件并进行retransmission rate的计算。

*client.py*：通信端的抽象。实现了一个sender、receiver的基本功能。

*config.ini*：配置文件，包含的参数具体见代码。

*PDU.py*：自定义了PDU的结构，实现了PDU的封装和信息提取。

*timer.py*：实现了计时器timer类。

*utils.py*：wrapper of socket send&receive。

*host.py*：模拟了通信一方的基本操作。首先确定是通信中的哪一方（本项目只实现了两个主机之间的通信），然后导入配置文件，最后输入要向对方发送的文件的相对路径名。
