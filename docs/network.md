## ubuntu 20.04 的server版本

  连接隐藏的wifi时
  需要修改/etc/netplan/00-installer-config-wifi.yaml

```bash
network:
  version: 2
  wifis:
    wlp0s20f3:
      dhcp4: yes
      optional: true
      access-points:
        qhx_ops:
          password: xxxxx
          hidden: true
```
