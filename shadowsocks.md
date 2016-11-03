## shadowsocks 服务端 ( centos 7 )
### 安装 yum 扩展源 ( EPEL 源 )
```
yum -y install epel-release
```
### 安装 pip
```
yum -y install python-pip
```
### 通过 pip 安装 shadowsocks
```
pip install shadowsocks
```
### 开启 shadowsocks 服务端
```
ssserver -s ::0 -p 58237 -k ODRlMDczND -m aes-256-cfb --user nobody --workers 2 -d start
```
---
---
## shadowsocks 客户端
### Windows 
#### [win客户端](https://github.com/shadowsocks/shadowsocks-windows/releases)
##### ( win 7 用 2.3 版本，win 10 用 3.0 版本 )
### Linux
#### [linux客户端](https://github.com/shadowsocks/shadowsocks-qt5)( 仅支持全局代理 ) 
```
yum update
yum install shadowsocks-qt5
```
### Mac
#### [Mac客户端](https://github.com/shadowsocks/shadowsocks-iOS/releases)