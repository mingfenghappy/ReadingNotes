# 第1章 了解Web及网络基础

讲了TCP/IP协议族,分层,如何传输,TCP三次握手,URI&URL等 

## TCP/IP 分层管理

TCP/IP协议族按层次分别分为以下4层:**应用层==>传输层==>网络层==>数据链路层**

###  应用层
应用层**决定了向用户提供应用服务时通信的活动**.

TCP/IP协议族内预存了各类通用的应用服务,如:`FTP` `DNS` `HTTP`

### 传输层
传输层对上层应用层,提供处于网络连接中的两台计算机之间的数据传输.  

传输层有两个不同的协议:`TCP`和`UDP`  

	PS: TCP 可靠 ,UDP 不可靠 后面会讲

### 网络层(又名网络互联层)

网络层用来**处理在网络上流动的数据包**. 数据包是网络传输的最小单位   

网络层所起的作用就是在众多的选项内选择一条传输路线  

**IP协议在网络层**

### 链路层(又名数据链路层,网络接口层)
用来处理链接网络的硬件部分    



## TCP 

TCP 位于传输层,提供**可靠的字节流服务**  

###  字节流服务 Byte Stream Service
字节流服务是指 **为了方便传输,将大块数据分割成以`报文段(segment)`为单位的数据包进行管理** 这样能更容易传送大数据  

### 可靠性(三次握手)
TCP的可靠性是因为它采用了**三次握手策略(three-way handshaking)**  

握手过程中使用了TCP的标志:  
- SYN(synchronize)
- ACK(acknowledgement 确认)

三次握手的过程:  

1. 客户端先发送带有

