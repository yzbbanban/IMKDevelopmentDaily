当然是 x86 架构编译...  

启用一下 TCP 代替 UDP, [lrinQVQ](https://github.com/lrinQVQ) 大神 说下载效果佳
``` bash
sudo sysctl -w net.ipv4.tcp_window_scaling=0
```
