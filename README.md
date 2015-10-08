# iptux: 飞鸽传书 GNU/Linux 版

[![Build Status](https://travis-ci.org/iptux-src/iptux.png?branch=master)](https://travis-ci.org/iptux-src/iptux)
[![GitHub version](https://badge.fury.io/gh/iptux-src%2Fiptux.png)](http://badge.fury.io/gh/iptux-src%2Fiptux)

* If anyone want to adopt this software, please [file an issue](https://github.com/iptux-src/iptux/issues/new)<br>
  at https://github.com/iptux-src/iptux/issues/new


## Install

### Linux (Debian and Ubuntu)

```
sudo apt-get install iptux
```


## Build from source

### Linux (Debian and Ubuntu)

```
sudo apt-get install git libgtk2.0-dev libgconf2-dev libgstreamer1.0-dev g++ make autoconf libtool automake
git clone git://github.com/iptux-src/iptux.git
cd iptux
./configure
make
sudo make install
iptux
```

### Mac OS X

```
brew install autoconf gettext gtk+ gconf
git clone git://github.com/iptux-src/iptux.git
cd iptux
./configure CPPFLAGS="-I/usr/local/opt/gettext/include" PKG_CONFIG_PATH=/opt/X11/lib/pkgconfig
make
sudo make install
iptux
```


## 贡献

* [Launchpad](http://translations.launchpad.net/iptux/trunk) 为 iptux 贡献翻译。页面由 LI Daobing &lt;lidaobing@gmail.com&gt; 提供；
* 欢迎为 iptux (最新版) 制作二进制包、提供补丁。

## 声明

请总是使用最新版本！！

* 老版本中出现的 bug 可能已被修正；
* 许多新特性需要您的试用。

## 基本

兼容 Windows 版[飞鸽传书](http://www.ipmsg.org.cn/)、[飞秋](http://www.feiq18.com/)和 Android 版飞鸽协议，也兼容日本<u>白水啓章</u>先生 (@shirouzu) 原著的 [IP Messenger](http://ipmsg.org/)，实现局域网的通信，文件传输。

## 提高

自定义一部分命令字，实现文件共享功能，群组通信，自动识别编码

## 相关
请查看 Wiki 标签，那里可能有你需要的内容！

## 必须

* 打开防火墙的 TCP/UDP 2425 端口
* 运行命令: `gconftool-2 --recursive-unset /apps/iptux` (使用时机: 从 <= 0.4.5 升级到 >= 0.5.0)
* 运行命令: `sudo gtk-update-icon-cache PREFIX/share/icons/hicolor` (使用时机: 图标显示异常，PREFIX 为程序安装目录)


## TODO
错误不可避免，请发送错误报告到 https://github.com/iptux-src/iptux/issues
