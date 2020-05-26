# shadowsocks搭建笔记

* 服务端安装命令：

wget --no-check-certificate -O shadowsocks.sh https://raw.githubusercontent.com/xllg/shadowsocks/master/shadowsocks.sh

chmod +x shadowsocks.sh

systemctl stop firewalld && systemctl disable firewalld （好像不用关闭防火墙）

./shadowsocks.sh 2>&1 | tee shadowsocks.log

* 客户端下载地址：

https://github.com/shadowsocks/shadowsocks-windows/releases

* 扩展命令：

启动：/etc/init.d/shadowsocks start

停止：/etc/init.d/shadowsocks stop

重启：/etc/init.d/shadowsocks restart

状态：/etc/init.d/shadowsocks status

配置文件路径：/etc/shadowsocks.json

卸载方法：/usr/local/src/shadowsocks.sh uninstall

