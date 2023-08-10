## Fabric服务端入门
**官网：https://fabricmc.net/**
* **安装JDK**
  * **下载JDK**  
https://www.oracle.com/cn/java/technologies/downloads/  
`D:\Administrator\Downloads\jdk-20_windows-x64_bin.exe`
  * **安装`jdk-20_windows-x64_bin.exe`**
  * **删除`jdk-20_windows-x64_bin.exe`（可选**
* **生成`server.properties`**
  * **下载服务端和API**  
https://fabricmc.net/use/server/  
`D:\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2\`
    * **下载服务端**  
`D:\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2.jar`
    * **下载API**  
`D:\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2\fabric-api-0.86.1+1.20.1.jar`
  * **运行`fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2.jar`生成`eula.txt`**  
`D:\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2\eula.txt`
  * **更改`eula.txt`**  
`D:\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2\eula.txt`
    ```
    eula=true
    ```
  * **新建`fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2.bat`，运行生成`server.properties`并关闭**
    ```
    java -Xmx2G -jar fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2.jar nogui
    ```
* **更改`server.properties`**  
`D:\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2\server.properties`
https://minecraft.fandom.com/zh/wiki/Server.properties
  ```
  allow-flight=true
  difficulty=hard
  gamemode=survival
  max-players=20
  motd=A Minecraft Server
  online-mode=true
  server-port=25565
  spawn-protection=0
  view-distance=10
  ```
* **下载`mods`**  
`D:\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2\mods\`
  * **移动`fabric-api-0.86.1+1.20.1.jar`到`mods`文件夹**  
`D:\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2\mods\fabric-api-0.86.1+1.20.1.jar`
    * **C<sup>2</sup>ME [ C<sup>2</sup>M引擎 ]**  
https://modrinth.com/mod/c2me-fabric
    * **Carpet**  
https://modrinth.com/mod/carpet
    * **Debugify**  
https://www.modrinth.com/mod/debugify
    * **EasyAuth**  
https://modrinth.com/mod/easyauth
    * **Fabric API**  
https://www.modrinth.com/mod/fabric-api
    * **Fastload**  
https://modrinth.com/mod/fastload
    * **FerriteCore [ 铁氧体磁芯 ]**  
https://modrinth.com/mod/ferrite-core
    * **Geyser**  
https://modrinth.com/mod/geyser
    * **Krypton [ 氪 ]**  
https://www.modrinth.com/mod/krypton
    * **LazyDFU [ DFU载入优化 ]**  
https://www.modrinth.com/mod/lazydfu
    * **Lithium [ 锂 ]**  
https://www.modrinth.com/mod/lithium
    * **Memory Leak Fix**  
https://modrinth.com/mod/memoryleakfix
    * **SkinRestorer**  
https://www.curseforge.com/minecraft/mc-mods/skinrestorer
    * **Starlight [ 星光 ]**  
https://modrinth.com/mod/starlight
    * **VMP**  
https://modrinth.com/mod/vmp-fabric
* **更改`EasyAuth` `config.json`**
  * **运行`fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2.bat`生成`EasyAuth`文件夹**  
`D:\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2\mods\EasyAuth`
  * **更改`config.json`**
    ```
    {
      "main": {
        "premiumAutologin": true
      }
    }
    ```


**To be continued...**