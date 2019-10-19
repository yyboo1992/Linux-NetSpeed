# Linux-NetSpeed
```
wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh"
chmod +x tcp.sh
./tcp.sh
```

启动命令 /appex/bin/lotServer.sh start
停止加速 /appex/bin/lotServer.sh stop
状态查询 /appex/bin/lotServer.sh status
重新启动 /appex/bin/lotServer.sh restart

Q&A
Q: 为何许可证有效期只有6个月?
A: 仅供学习和测试使用.

Q: 如何能够长期使用?
A: 请利用cron设置定时任务,以便自动更新许可证.

无法使用需要更新许可   第一次也需要
Q: 如何更新许可证?
A: 使用 ifconfig 查看网卡 mac 地址, 替换 00:00:00:00:00:00 ,当版本号小于等于 3.11.20.10 时, 请设置 ver=0 .

wget --no-check-certificate -qO '/appex/etc/apx.lic' "https://api.moeclub.org/lotServer?ver=1&mac=00:00:00:00:00:00" 
