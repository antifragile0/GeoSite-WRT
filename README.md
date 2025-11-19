## **RTA SERVER**：

## Best Rule Clash Meta - Mihomo - SingBox Generator

## **country.mmdb,geoip.dat,geoip.db**

- Cara penggunaannya sama dengan [Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)  

| country.mmdb,geoip.dat |
| ---------------- |
| `geoip:id` **Routing Indonesia Only**| 
| `geoip:cloudflare` |
| `geoip:cloudfront` | 
| `geoip:facebook` | 
| `geoip:netflix` |
| `geoip:telegram` | 
| `geoip:twitter` | 

| Name Content | Link Download |
| ------------ | ------------- |
| **country.mmdb** | [Github release](https://github.com/antifragile0/GeoSite-WRT/releases/download/latest/country.mmdb) - [JSdelivr](https://cdn.jsdelivr.net/gh/antifragile0/GeoSite-WRT@release/country.mmdb) - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/antifragile0/GeoSite-WRT@release/country.mmdb) |
| **geoip.dat** | [Github release](https://github.com/antifragile0/GeoSite-WRT/releases/download/latest/geoip.dat) - [JSdelivr](https://cdn.jsdelivr.net/gh/antifragile0/GeoSite-WRT@release/geoip.dat) - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/antifragile0/GeoSite-WRT@release/geoip.dat) |
| **geoip.db** | [Github release](https://github.com/antifragile0/GeoSite-WRT/releases/download/latest/geoip.db) - [JSdelivr](https://cdn.jsdelivr.net/gh/antifragile0/GeoSite-WRT@release/geoip.db) - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/antifragile0/GeoSite-WRT@release/geoip.db) |
| **geoip.metadb** | [Github release](https://github.com/antifragile0/GeoSite-WRT/releases/download/latest/geoip.metadb) - [JSdelivr](https://cdn.jsdelivr.net/gh/antifragile0/GeoSite-WRT@release/geoip.metadb) - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/antifragile0/GeoSite-WRT@release/geoip.metadb) |

## **geosite.dat,geosite.db**

- Cara penggunaannya sama dengan [Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)  

| geosite.dat,geosite.db |
| ---------------- |
|  `geosite:rule-ads` |
|  `geosite:rule-doh` |
|  `geosite:rule-gaming` |
|  `geosite:rule-indo` |
|  `geosite:rule-playstore` |
|  `geosite:rule-sosmed` |
|  `geosite:rule-streaming` |
|  `geosite:rule-umum` |
|  `geosite:rule-ipcheck` |
|  `geosite:rule-speedtest` |
|  `geosite:videoconference` |
|  `geosite:urltest` |
|  `geosite:bank-id` |


| Name Content | Link Download |
| ------------ | ------------- |
| **geosite.dat** | [Github release](https://github.com/antifragile0/GeoSite-WRT/releases/download/latest/geosite.dat) - [JSdelivr](https://cdn.jsdelivr.net/gh/antifragile0/GeoSite-WRT@release/geosite.dat) - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/antifragile0/GeoSite-WRT@release/geosite.dat) |
| **geosite.db** | [Github release](https://github.com/antifragile0/GeoSite-WRT/releases/download/latest/geosite.db) - [JSdelivr](https://cdn.jsdelivr.net/gh/antifragile0/GeoSite-WRT@release/geosite.db) - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/antifragile0/GeoSite-WRT@release/geosite.db) |

---
## Install & Update

### Use Auto Script
- Wget
```shell
bash -c "$(wget -qO - 'https://github.com/antifragile0/GeoSite-WRT/raw/refs/heads/master/main.sh')"
```
- Curl
```shell
bash -c "$(curl -fsSL 'https://github.com/antifragile0/GeoSite-WRT/raw/refs/heads/master/main.sh')"
```

---

## **OpenClash-Meta**

[Download Full Config Meta](https://github.com/antifragile0/Config-Open-ClashMeta?tab=readme-ov-file#----config-openclash---meta-kernel)
```yaml

rules:
- DST-PORT,7895,REJECT
- DST-PORT,7892,REJECT
- IP-CIDR,198.18.0.1/16,REJECT,no-resolve
#- AND,((GEOSITE,rule-ads),(NOT,((DOMAIN-SUFFIX,googlesyndication.com)))),REJECT
- RULE-SET,Direct,DIRECT
- RULE-SET,UDP,UDP-Traffic
#- RULE-SET,Pilih,PILIH
- RULE-SET,Khusus,Bandwidth
- GEOSITE,bank-id,Indo-Traffic
- GEOSITE,rule-indo,Indo-Traffic
- GEOSITE,rule-sosmed,Indo-Traffic
- GEOSITE,rule-streaming,Indo-Traffic
- GEOSITE,rule-gaming,UDP-Traffic
- GEOSITE,rule-speedtest,PILIH
- GEOSITE,urltest,Ping-Alive
- MATCH,GLOBAL
```

## Thangks To

- [@Loyalsoldier/geoip](https://github.com/Loyalsoldier/geoip)
- [@v2fly/domain-list-community](https://github.com/v2fly/domain-list-community)
- [@Loyalsoldier/domain-list-custom](https://github.com/Loyalsoldier/domain-list-custom)
- [@felixonmars/dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list)
- [@gfwlist/gfwlist](https://github.com/gfwlist/gfwlist)
- [@cokebar/gfwlist2dnsmasq](https://github.com/cokebar/gfwlist2dnsmasq)
- [@Loyalsoldier/cn-blocked-domain](https://github.com/Loyalsoldier/cn-blocked-domain)
- [@AdblockPlus/EasylistChina+Easylist.txt](https://easylist-downloads.adblockplus.org/easylistchina+easylist.txt)
- [@AdGuard/DNS-filter](https://kb.adguard.com/en/general/adguard-ad-filters#dns-filter)
- [@PeterLowe/adservers](https://pgl.yoyo.org/adservers)
- [@DanPollock/hosts](https://someonewhocares.org/hosts)
- [@crazy-max/WindowsSpyBlocker](https://github.com/crazy-max/WindowsSpyBlocker)
- [@blackmatrix7/ios_rule_script](https://github.com/blackmatrix7/ios_rule_script)
- [@malikshi/v2ray-rules-dat](https://github.com/malikshi/v2ray-rules-dat)
