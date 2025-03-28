# NetCheater-wuhues

## ⚠️ 警告
**本项目仅用于教育目的和网络安全研究！**
- 未经授权使用本工具获取他人账号信息是违法行为
- 使用本工具进行网络攻击可能导致严重的法律后果
- 作者不对任何滥用本工具的行为负责

## 功能特点
- 基于 ESP32-S3 实现
- 创建名为"School-Wifi"的无线接入点
- 提供与校园网完全一致的登录页面
- 捕获并记录用户输入的账号和密码信息

## 硬件要求
- ESP32-S3 开发板
- 电源供应（USB或电池）
- （可选）SD卡用于存储更多日志

## 软件依赖
- Arduino IDE
- ESP32-S3 Arduino 核心库
- 以下Arduino库:
  - WiFi.h
  - DNSServer.h
  - WebServer.h
  - SPIFFS.h

## 安装使用
1. 克隆本仓库到本地
   ```
   git clone https://github.com/Shiqi-SQ/NetCheater-wuhues.git
   ```
2. 在Arduino IDE中打开`NetCheater_wuhues.ino`文件
3. 安装所需的库和依赖
4. 将ESP32-S3连接到计算机
5. 编译并上传代码到ESP32-S3
6. 设备启动后，将广播"School-Wifi"热点

## 工作原理
1. ESP32-S3创建一个开放的WiFi热点，名称为"School-Wifi"
2. 当用户连接到这个热点后，无论访问什么网址，都会被重定向到仿冒的登录页面
3. 用户输入账号密码后，这些信息会被记录在设备上
4. 可通过串口监视器或Web界面查看捕获的凭据

## 免责声明
本项目仅供学习和研究网络安全知识，请勿用于非法目的。使用本工具进行未授权的网络活动可能违反相关法律法规。作者不对任何滥用本工具的行为负责。
