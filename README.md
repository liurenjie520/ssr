# ssr


 http://www.vultr.com
 
 CentOS6/Debian6/Ubuntu14 ShadowsocksR一键部署管理脚本：
 
yum -y install wget

wget -N --no-check-certificate https://raw.githubusercontent.com/liurenjie520/ssr/master/ssr.sh && chmod +x ssr.sh && bash ssr.sh
 
 
备用脚本： 
 

yum -y install wget

wget -N --no-check-certificate https://raw.githubusercontent.com/ToyoDAdoubi/doubi/master/ssr.sh && chmod +x ssr.sh && bash ssr.sh




# 快捷管理命令bash ssr.sh启动ssr管理


注意：如果协议是origin，那么混淆也必须是plain；如果协议不是origin，那么混淆可以是任意的。
有的地区需要把混淆设置成plain才好用。因为混淆不总是有效果，要看各地区的策略，有时候不混淆（plain）让其看起来像随机数据更好。
（特别注意：tls 1.2_ticket_auth容易受到干扰！请选择除tls开头以外的其它混淆！！！）



进行混淆插件的设置后，会依次提示你对设备数、单线程限速和端口总限速进行设置，默认值是不进行限制，个人使用的话，选择默认即可，即直接敲回车键。

注意：关于限制设备数，这个协议必须是非原版且不兼容原版才有效，也就是必须使用SSR协议的情况下，才有效！


此脚本是开机自动启动，部署一次即可。最后可以重启服务器确保部署生效（一般情况不重启也可以）。
重启需要在命令栏里输入reboot ，输入命令后稍微等待一会服务器就会自动重启，一般重启过程需要2～5分钟，重启过程中Xshell会自动断开连接，等VPS重启好后才可以用Xshell软件进行连接。
如果部署过程中卡在某个位置超过10分钟，可以用xshell软件断开，然后重新连接你的ip，再复制代码进行部署。


# 一键加速VPS服务器

登录成功后，在命令栏里粘贴以下代码：

【谷歌BBR加速教程】

yum -y install wget

wget --no-check-certificate https://raw.githubusercontent.com/liurenjie520/ssr/master/bbr.sh

chmod +x bbr.sh

./bbr.sh


备用脚本：

yum -y install wget

wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh

chmod +x bbr.sh

./bbr.sh

把上面整个代码复制后粘贴进去，不动的时候按回车，然后耐心等待，最后重启vps服务器即可。
按任意键继续部署

最后输入y重启服务器，如果输入y提示command not found ，接着输入reboot来重启服务器，确保加速生效，bbr加速脚本是开机自动启动，装一次就可以了。


服务器重启成功并重新连接服务器后，输入命令lsmod | grep bbr 如果出现tcp_bbr字样表示bbr已安装并启动成功。




# 【SSR客户端下载】

第一次电脑系统使用SSR/SS客户端时，如果提示你需要安装NET Framework 4.0，网上搜一下这个东西，安装一下即可。NET Framework 4.0是SSR/SS的运行库，没有这个SSR/SS客户端无法正常运行。有的电脑系统可能会自带NET Framework 4.0。

Windows SSR客户端 https://github.com/shadowsocksr-backup/shadowsocksr-csharp/releases

MAC SSR客户端 https://github.com/shadowsocksr-backup/ShadowsocksX-NG/releases

安卓SSR客户端 https://github.com/shadowsocksr-backup/shadowsocksr-android/releases

苹果手机SSR客户端：Potatso Lite、Potatso、shadowrocket都可以作为SSR客户端，但这些软件目前已经在国内的app商店下架，
可以用美区的appid账号来下载。但是，如果你配置的SSR账号兼容SS客户端，或者协议选择origin且混淆选择plain，
那么你可以选择苹果SS客户端软件（即协议和混淆可以不填），APP商店里面有很多，
比如：superwingy、firstwingy、shadowingy、wingy+、banananet、kite-ss proxy、goodshadow、icproyx、shadowrocket等。
