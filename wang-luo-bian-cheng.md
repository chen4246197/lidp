#网络编程
##基本概念
> * 注意：**网络编程涉及的是网络底层数据的传输**，
    是网页服务的底层（数据的传输原理，不同计算机数据的交流等）
    网页编程涉及的是与客户的交互，就是网页排版（前端）。
    
###网络：不同计算机连接所构成的网络（简单说）
 ●局域网
 ●城域网
 ●互联网（万维网）
 
> * 地址：一般网络编程指IP地址。即是通讯设备的绝对位置地址（如房屋详细地址） 



***
![](/assets/wlbc1.png)
***
###端口号：如上图为了区分计算机软件做的标识地址（如门房号）。
> *端口号是由2字节标识（即0-65535以内的数字表示）
●在同一个协议（TCP/UDP）下端口号不能重复。不同的协议下可以重复。
> *端口号因为要预留操作系统本地程序，需要留1024以内的端口号不可使用
> *＞例如端口号80  留给http，端口号21留给ftg用的（例如电话号码110已经留给公共机关使用）

***
![](/assets/wlbc2.png)
***

###资源定位：如上图
 ####URL（Uniform Resource Locator）:统一资源定位符，通过这个命令符进行资源定位。
> *  ●协议：
 > * ●存放资源的主机域名：
 > * ●端口：
 > * ●资源端口名：
> * URI（Uniform Resource Identifier） 统一资源，
 
####数据的传输：
> *●●●协议：即通讯的规则。(重点)
> *CTP协议：类似我们打电话，必须建立连接才能进行数据连接（三次握手）.面向连接，安全可靠。效率相对UCP低下。
> *UDP协议：类似我们发短信,对讲机，面向无连接，安全性低，效率高。

***
![](/assets/wlbc3.png)
***
####数据如何传输：先封装后封装。
####网络编程所用的类
####IP地址类InetAdress：
>封装计算机的IP地址和DNS(域名解析即对www.XXX.com翻译为数字地址)，没有端口。
>方法：getHostAddress()：返回ip地址
>         getHostName()：返回域名
>端口号地址：InetSocketAddressn封装了端口
>  	 方法：getPort():返回端口号。

####资源定位类 URL
####TCP协议类ServerSocket 、Server。（传输控制协议）
####UDP协议类DatagramSocket、DatagramPacket（用户数据报协议）


>相对路径：相对于某个基准目录路径（一般相对于JVM路径）
>绝对路径：在文件或者硬盘上本地文件的不会更改的路径。
>★★★查询本机IP地址命令符cmd ipconfig/all