# OpenWrt Guides

* [Asignar boca WAN con Openwrt (Amper-ASL-26555)](http://openwrt.tuinstituto.es/asignar-boca-wan-con-openwrt-amper-asl-26555)
* [Wireless Router with a 3G/UMTS/HSDPA dongle](]https://josefsson.org/openwrt/dongle.html)
* [Modem: M-Life ML0700 LTE modem, with Qualcomm MDM9200 chipset](https://forum.openwrt.org/t/solved-3g-lte-modem-qualcomm-mdm9200-usb-modeswitch-problem/26730/7)

# OpenWrt on Linksys E5400 Router  
 
* [Installing OpenWRT onto Linksys E5400](https://farazkaleemmalik.cyou/blog/2023/openwrt1/)
* [Setting up a WireGuard server on OpenWRT](https://birkhoff.me/articles/setting-up-a-wireguard-server-on-openwrt)
* [Cómo configurar el router de Movistar en modo bridge](https://naseros.com/2017/08/03/como-configurar-el-router-de-movistar-en-modo-bridge/)
* [OpenWrt: Configuración VLans en router WRT3200ACM para O2](https://elblogdelazaro.org/posts/2019-06-24-configuraci%C3%B3n_vlans_en_router_wrt3200acm_para_o2/)

# Enable UART 1 in Beaglebone Black

I enabled the TX and RX pins for UART 1 with:

sudo config-pin P9.24 uart
sudo config-pin P9.26 uart

screen /dev/ttyS1 115200

Para salir de 'screen' pulsar: Ctrl-a + x

# Tailscale

* [How to Set Up Tailscale on OpenWrt](https://www.wundertech.net/how-to-set-up-tailscale-on-openwrt/) 