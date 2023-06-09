

#### 安装流程

- CMD
```
sudo apt-get update
sudo apt-get install snort -y
```
- 配置网卡: eth0
- Adress Range: 172.16.1.0/24
- Interfaces: Span

- √ 混杂模式/Promiscuous Mode = Alow
- × V-Box ```sudo ip link set ens0 promisc on```

#### 配置Snort

1. Tree
   - rules
   - snort.conf
2. Vim snort.conf
   1. set the network
     - HOME_NET 172.16.1.0/24
     - EXTERNAL_NET ANY
     - Any Server
   2.  Path to rules files
   3.  Customize Rules
   4.  Output
3. Test
4. 
