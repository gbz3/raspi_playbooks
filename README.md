# raspi_playbooks

## 事前設定
### 固定IP設定
~~~
pi@raspberrypi:~ $ sudo cp -p /etc/dhcpcd.conf /etc/dhcpcd.conf.20180520
pi@raspberrypi:~ $ sudo vi /etc/dhcpcd.conf
pi@raspberrypi:~ $ diff /etc/dhcpcd.conf /etc/dhcpcd.conf.20180520
46,49d45
< interface eth1
< static ip_address=192.168.10.254/24
< static routers=192.168.0.1
< static domain_name_servers=8.8.8.8
~~~

### リブート
~~~
pi@raspberrypi:~ $ shutdown -r now
~~~
