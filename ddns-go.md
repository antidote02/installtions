## DDNS-GO入门
**项目：https://github.com/jeessy2/ddns-go**  
* **下载DDNS-Go**  
https://github.com/jeessy2/ddns-go/releases  
`D:\ddns-go.exe`
* **启动DDNS-Go**
  * **双击**  
`D:\ddns-go.exe`
  * **安装服务（可选**  
`> D:\ddns-go.exe -s install`
* **升级DDNS-Go**  
`> D:\ddns-go.exe -s uninstall`  
替换`ddns-go.exe`  
`> D:\ddns-go.exe -s install`
* **前端**  
http://localhost:9876/
* **获取DDNS**
  * **Dynv6**  
https://dynv6.com/
    * **新建域**名  
https://dynv6.com/zones/new  
`Name` 必填  
`IPv4 Address` / `IPv6 prefix` 选填/不填  
例如：`yourhost.v6.navy`
    * **获取Token**  
https://dynv6.com/docs/apis  
在页面上查找`token=*`；复制`token=*`
    * http://localhost:9876/
      * `DNS服务商` `Callback`  
`URL` `http://dynv6.com/api/update?hostname=#{domain}&token=*&ipv6=#{ip}` 注意 `*`  
`TTL` `自动`
      * `IPV6` `启用`  
`获取IP方式` `通过接口获取`  
`Domains` `yourhost.v6.navy`
      * `Save`
* **卸载DDNS-Go服务**  
`> D:\ddns-go.exe -s uninstall`