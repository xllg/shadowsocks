# shadowsocks一键安装脚本笔记

安装命令：
=========

wget --no-check-certificate -O shadowsocks.sh https://raw.githubusercontent.com/xllg/shadowsocks/master/shadowsocks.sh

chmod +x shadowsocks.sh

systemctl stop firewalld && systemctl disable firewalld

./shadowsocks.sh 2>&1 | tee shadowsocks.log

扩展命令：
=========

启动：/etc/init.d/shadowsocks start

停止：/etc/init.d/shadowsocks stop

重启：/etc/init.d/shadowsocks restart

状态：/etc/init.d/shadowsocks status

配置文件路径：/etc/shadowsocks.json

卸载方法：/usr/local/src/shadowsocks.sh uninstall

