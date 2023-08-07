## Alist入门
**官网：https://alist.nn.ci/zh/**
### 后端
* **安装Scoop**  
https://learn.microsoft.com/zh-cn/previous-versions/windows/powershell-scripting/hh847748(v=wps.640)
https://github.com/ScoopInstaller/Install  
`Set-ExecutionPolicy Bypass`  
`cd D:\Administrator\Downloads`  
`irm get.scoop.sh -outfile 'install.ps1'`  
`.\install.ps1 -RunAsAdmin -ScoopDir 'D:\Applications\Scoop' -ScoopGlobalDir 'D:\GlobalScoopApps' -NoProxy`  
`rm install.ps1`
  * **设置代理**  
`scoop config proxy localhost:7890`/`scoop config rm proxy`
  * **添加Bucket**  
`scoop bucket known`  
`scoop bucket add extras`  
`scoop bucket add versions`  
`scoop bucket add nirsoft`  
`scoop bucket add sysinternals`  
`scoop bucket add php`  
`scoop bucket add nerd-fonts`  
`scoop bucket add nonportable`  
`scoop bucket add java`  
`scoop bucket add games`  
`scoop bucket add dorado https://github.com/chawyehsu/dorado`
  * **升级/删除缓存**  
`scoop install -k git`  
`scoop update -k *`  
`scoop cache rm *`
  * **卸载**  
`scoop uninstall scoop`
* **安装Alist**  
`scoop install -k alist`
* **获得管理员信息**  
`alist admin`
* **启动Alist**
  * **手动**  
启动程序/通过Pid重启服务  
`alist restart`  
通过pid停止服务  
`alist stop`
  * **`.vbs脚本`**  
新建`Alist启动.vbs`
    ```
    Dim ws
    Set ws = Wscript.CreateObject("Wscript.Shell")
    ws.run "alist.exe restart",0
    Wscript.quit
    ```
    新建`Alist停止.vbs`
    ```
    Dim ws
    Set ws = Wscript.CreateObject("Wscript.Shell")
    ws.run "taskkill /f /im alist.exe",0
    Wscript.quit
    ```
### 前端
* 主页  
http://localhost:5244/  
* 添加存储  
https://alist.nn.ci/zh/guide/drivers/

**以上。欢迎补充和指正**

![]()