# SingboxUnlockChatGPT


1. use singbox script to install Proxy
   https://233boy.com/sing-box/sing-box-script/
     bash <(wget -qO- -o- https://github.com/233boy/sing-box/raw/main/install.sh)

optional: 
   enable bbr
    ```
    echo net.core.default_qdisc=fq >> /etc/sysctl.conf

   
    echo net.ipv4.tcp_congestion_control=bbr >> /etc/sysctl.conf
    sysctl -p
    lsmod | grep bbr
    ```

2. install cloudflare warp to unlock chatgpt
  https://p3terx.com/archives/cloudflare-warp-configuration-script.html
  bash <(curl -fsSL git.io/warp.sh) d
