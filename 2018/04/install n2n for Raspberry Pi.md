树莓派上安装N2N 实现NAT穿透
===




## 准备工作
1. 一台有外网的
```Shell
supernode -l 9000 #UDP监听端口 
 
#参数说明
-f 前台运行
-u 指定运行所用的UID
-g 指定运行所用的GID
-v 输出比较详细的log
```

```Bash
edge -d 虚拟网卡名 -a 10.0.0.1 -c testnet -k senrame -l 1.2.3.4:1234
 
#参数说明
-d 虚拟网卡名
-a [static:|dhcp:]虚拟网段(IP)，static模式其实可以不用加那个static: 直接写IP就行
-c 用于区分节点的社区(组)名
-k 用于加密的字符串
-K 用于加密的Key文件，和-k不能共存
-s 子网掩码
-l supernode的IP:端口，可以指定多个supernode的
-i NAT打洞间隔
-b 当使用DHCP时定期刷新IP
-p 指定本地端口
-u 指定运行所用的UID
-g 指定运行所用的GID
-f 前台运行
-m 为虚拟网卡指定MAC地址
-r 启用包转发，当-a指定DHCP时需要启用
-E 接收组播MAC地址
-v 输出比较详细的log
-t 指定用于管理的UDP端口

```


## 参考链接

[meyerd/n2n](https://github.com/meyerd/n2n)

[P2P网络-n2n穿墙](http://gohom.win/2016/09/03/n2n-p2pnet/)

[重新编译N2N](http://blog.51cto.com/yuanhuan/1720811)

[内网穿透系列——N2N（简单的P2P组网方案）](http://www.senra.me/nat-traversal-series-n2n-a-easy-p2p-vpn-solution/)

[组建N2N VPN网络实现内网设备之间的相互访问
](https://www.shuyz.com/posts/n2n-vpn-network-introduction-and-config/)