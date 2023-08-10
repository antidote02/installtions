## Fabric服务端入门
**官网：https://fabricmc.net/**
* **安装JDK**
  * **下载JDK**  
https://www.oracle.com/cn/java/technologies/downloads/  
`D:\Administrator\Downloads\jdk-20_windows-x64_bin.exe`
  * **安装`jdk-20_windows-x64_bin.exe`并删除**
* **生成`server.properties`**
  * **下载服务端**  
https://fabricmc.net/use/server/  
`D:\Administrator\Downloads\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2.jar`
  * **新建`fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2`文件夹**  
`D:\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2`
  * **移动`fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2.jar`到`fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2`文件夹**  
`D:\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2.jar`
  * **运行`fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2.jar`生成`eula.txt`**  
`D:\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2\eula.txt`
  * **更改`eula.txt`**  
`D:\fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2\eula.txt`
    ```
    eula=true
    ```
  * **新建`fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2.bat`，运行，并关闭**
    ```
    java -Xmx2G -jar fabric-server-mc.1.20.1-loader.0.14.22-launcher.0.11.2.jar nogui
    ```
* **更改`server.properties`**  
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

**To be continued...**