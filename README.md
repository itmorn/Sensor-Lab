# SensorMuseum | 传感器博物馆

https://img.shields.io/badge/License-MIT-blue.svg](LICENSE)
https://img.shields.io/badge/Docs-Read%20Online-brightgreen](https://sensor-museum.readthedocs.io/)
https://img.shields.io/badge/Bilibili-关注-green](https://space.bilibili.com/YOUR_ID)
https://img.shields.io/badge/YouTube-订阅-red](https://youtube.com/YOUR_CHANNEL)

> 一个由算法工程师兼嵌入式开发者精心整理的传感器与执行器实战知识库

欢迎来到**传感器博物馆**！我是一个有着"收藏癖"的算法工程师，致力于为硬件爱好者建立一个**系统化、可复用**的传感器与执行器知识库。这里不仅有原理讲解、代码实现，更有完整的项目和优化技巧。

## 📋 目录

- #-项目理念
- #-项目结构
- #-传感器模块
  - #️-温湿度传感器
  - #-光敏与环境光传感器
  - #-运动与姿态传感器
  - #-距离与接近传感器
  - #️-气体与空气质量传感器
  - #-触摸与按键
- #️-执行器模块
  - #-电机与驱动
  - #-显示模块
  - #-声音与发声
  - #-开关与继电器
- #-通信与协议
  - #-有线通信
  - #-无线通信
- #️-实战项目
  - #-智能家居系列
  - #-机器人系列
  - #-环境监测系列
- #-进阶内容
  - #️-信号处理与算法
  - #-电源管理与低功耗
  - #-数据处理与可视化
- #-快速开始
- #-参与贡献
- #-许可证
- #-联系与支持

## 🎯 项目理念

> "理解原理 → 掌握代码 → 创造项目"

作为一名算法工程师，我深知**理论与实践结合**的重要性。这个项目的目标是：

1. **系统化学习** - 从物理原理到代码实现，建立完整的知识体系
2. **收藏级完整** - 不满足于单个模块，追求同一类别的完整对比
3. **可重复使用** - 每个模块都有完整、可独立运行的代码示例
4. **持续更新** - 随着新技术的出现不断更新内容

## 📁 项目结构

```
sensor-museum/
├── docs/                          # 详细文档
│   ├── sensors/                   # 传感器文档
│   ├── actuators/                 # 执行器文档
│   ├── protocols/                 # 通信协议文档
│   └── projects/                  # 项目文档
├── examples/                      # 代码示例
│   ├── arduino/                   # Arduino平台示例
│   ├── stm32/                     # STM32平台示例
│   ├── esp32/                     # ESP32平台示例
│   └── raspberry-pi/              # 树莓派平台示例
├── libraries/                     # 自定义库文件
│   ├── sensor-lib/                # 传感器驱动库
│   ├── actuator-lib/              # 执行器驱动库
│   └── utils/                     # 工具函数库
├── projects/                      # 完整项目
│   ├── smart-home/                # 智能家居项目
│   ├── robot-car/                 # 智能小车项目
│   └── weather-station/           # 气象站项目
├── hardware/                      # 硬件设计文件
│   ├── schematics/                # 电路原理图
│   ├── pcb/                       # PCB设计文件
│   └── 3d-models/                  # 3D打印模型
├── tutorials/                     # 视频教程配套资料
├── tests/                         # 测试代码
└── resources/                     # 资源文件
    ├── datasheets/                # 数据手册
    └── references/                # 参考文档
```

## 🔧 传感器模块

### 🌡️ 温湿度传感器
- **DHT11/DHT22** - 入门级温湿度传感器的对比与深度解析
- **SHT3x系列** - 工业级精度温湿度传感器的应用
- **BME280/BMP280** - 集成温湿度气压三合一传感器
- **DS18B20** - 单总线数字温度传感器
- **AHT20** - 新一代高精度温湿度传感器
- docs/sensors/temperature-humidity/

### 💡 光敏与环境光传感器
- **光敏电阻** - 基础光敏元件原理与应用
- **BH1750** - 数字光照强度传感器
- **TSL2561/TSL2591** - 高精度光照传感器
- **APDS-9960** - 集成手势、接近、光感、RGB的传感器
- **VEML7700** - 超高精度环境光传感器
- docs/sensors/light/

### 🔄 运动与姿态传感器
- **MPU6050** - 六轴陀螺仪加速度计（含DMP使用）
- **MPU9250** - 九轴运动传感器
- **BNO055** - 自带融合算法的姿态传感器
- **LSM6DS3/LSM6DSL** - 低功耗高精度IMU
- **姿态融合算法** - 互补滤波、卡尔曼滤波、Mahony算法
- docs/sensors/motion/

### 📏 距离与接近传感器
- **HC-SR04** - 超声波测距模块
- **VL53L0X/VL53L1X** - 激光测距传感器
- **TCRT5000** - 红外反射式传感器
- **GP2Y0A21YK0F** - 红外测距传感器
- **RCWL-0516** - 微波雷达人体感应模块
- docs/sensors/distance/

### 🌫️ 气体与空气质量传感器
- **MQ系列** - 可燃气体、空气质量传感器家族
- **CCS811** - 室内空气质量传感器（eCO2, TVOC）
- **SGP30/SGP40** - 气体多像素传感器
- **PMS5003** - 激光粉尘传感器
- **SGP30** - 金属氧化物气体传感器
- docs/sensors/gas/

### 👆 触摸与按键
- **TTP223** - 电容式触摸开关
- **TTP229** - 16键电容触摸芯片
- **矩阵键盘** - 4x4矩阵键盘原理与应用
- **旋转编码器** - EC11旋转编码器的使用
- **触摸滑条** - 线性电容触摸传感器
- docs/sensors/touch/

## ⚙️ 执行器模块

### 🚗 电机与驱动
- **直流电机** - 基础驱动与控制
- **L298N驱动模块** - 经典双H桥电机驱动
- **TB6612FNG** - 更高效的直流电机驱动
- **28BYJ-48步进电机** - 五线四相步进电机
- **A4988/DRV8825** - 步进电机驱动模块
- **SG90/MG996R舵机** - PWM舵机控制
- docs/actuators/motors/

### 📺 显示模块
- **LED与RGB LED** - 基础发光器件控制
- **数码管** - 7段数码管与TM1637驱动
- **0.96寸OLED** - SSD1306驱动的OLED屏
- **LCD1602/2004** - 字符型液晶显示屏
- **TFT彩屏** - ILI9341驱动的彩色屏幕
- **WS2812B** - 可编程RGB LED灯带
- docs/actuators/display/

### 🔊 声音与发声
- **有源/无源蜂鸣器** - 发声原理与音乐播放
- **喇叭与功放** - LM386音频放大电路
- **DFPlayer Mini** - MP3播放模块
- **语音合成模块** - SYN6288语音播报
- docs/actuators/sound/

### 🔌 开关与继电器
- **电磁继电器** - SRD-05VDC继电器模块
- **固态继电器** - SSR固态继电器
- **MOSFET开关** - 大功率MOSFET控制
- docs/actuators/relay/

## 🔌 通信与协议

### 📡 有线通信
- **UART/串口通信** - 基础串行通信协议
- **I2C总线** - 两线制通信协议
- **SPI总线** - 高速全双工通信协议
- **1-Wire总线** - 单总线通信协议
- **CAN总线** - 工业现场总线
- docs/protocols/wired/

### 📶 无线通信
- **蓝牙** - HC-05/HC-06蓝牙模块
- **蓝牙低功耗** - HM-10 BLE模块
- **WiFi** - ESP8266/ESP32 WiFi通信
- **LoRa** - SX1278 LoRa模块
- **RFID/NFC** - RC522 RFID读写模块
- docs/protocols/wireless/

## 🛠️ 实战项目

### 🏠 智能家居系列
- **智能灯光系统** - 光感+触摸+RGB LED+WiFi控制
- **环境监测站** - 多传感器+OLED显示+数据上传
- **自动浇花系统** - 土壤湿度+继电器+水泵控制
- **智能窗帘** - 光感+电机+定时控制
- **安防监控系统** - 人体感应+摄像头+报警
- projects/smart-home/

### 🚗 机器人系列
- **循迹避障小车** - 红外+超声波+电机控制
- **蓝牙遥控车** - 手机APP+蓝牙控制
- **视觉巡线车** - 摄像头+OpenMV图像识别
- **机械臂** - 多舵机控制+逆运动学
- projects/robotics/

### 🌍 环境监测系列
- **便携式气象站** - 多传感器+太阳能供电
- **室内空气质量监测仪** - 多气体传感器+数据显示
- **水质监测浮标** - pH值+浊度+温度监测
- **噪声监测仪** - 声音传感器+数据记录
- projects/environment/

## 📈 进阶内容

### 🎛️ 信号处理与算法
- **数据滤波算法** - 移动平均、中值滤波、卡尔曼滤波
- **传感器校准** - 零位校准、灵敏度校准、温漂补偿
- **PID控制算法** - 位置式PID、增量式PID
- **运动融合算法** - 互补滤波、Mahony、Madgwick算法
- docs/advanced/signal-processing/

### 🔋 电源管理与低功耗
- **电池管理** - 锂电池充放电保护
- **DC-DC转换** - 升降压电路设计
- **低功耗设计** - 休眠模式、间歇工作
- **电源完整性** - 去耦、滤波、稳压
- docs/advanced/power-management/

### 📊 数据处理与可视化
- **数据记录** - SD卡存储、EEPROM存储
- **数据可视化** - 串口绘图、OLED绘图
- **上位机开发** - Python GUI、手机APP
- **云端数据** - MQTT、HTTP API、数据库
- docs/advanced/data-visualization/

## 🚀 快速开始

### 1. 环境准备
```bash
# 克隆仓库
git clone https://github.com/yourname/sensor-museum.git
cd sensor-museum

# 安装依赖（根据平台选择）
# Arduino用户：安装对应库文件
# STM32用户：安装STM32CubeIDE或PlatformIO
# ESP32用户：安装ESP-IDF或Arduino Core
```

### 2. 第一个示例
查看最简单的LED闪烁示例：
```c
// examples/arduino/basics/01-blink/01-blink.ino
void setup() {
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop() {
  digitalWrite(LED_BUILTIN, HIGH);
  delay(1000);
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000);
}
```

### 3. 学习路径建议
1. **初学者**：从 `docs/` 中的基础传感器开始
2. **中级用户**：参考 `examples/` 中的代码示例
3. **进阶用户**：尝试 `projects/` 中的完整项目
4. **贡献者**：查看开发指南，提交你的代码

## 🤝 参与贡献

我们欢迎任何形式的贡献！无论你是发现了一个bug，有改进建议，还是想添加新的传感器教程，都欢迎参与。

### 贡献流程
1. Fork 本仓库
2. 创建你的分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启一个 Pull Request

### 贡献指南
- 确保你的代码有清晰的注释
- 更新相关的文档
- 添加必要的测试
- 遵循现有的代码风格

## 📄 许可证

本项目采用 MIT 许可证 - 查看 LICENSE 文件了解详情。

## 📧 联系与支持

- **📺 视频教程**：https://space.bilibili.com/YOUR_ID | https://youtube.com/YOUR_CHANNEL
- **💬 技术交流**：https://jq.qq.com/?_wv=1027&k=YOUR_KEY | https://t.me/YOUR_GROUP
- **📧 邮件联系**：your.email@example.com
- **🐦 社交媒体**：https://twitter.com/YOUR_ID | https://weibo.com/YOUR_ID

---
<div align="center">
  <sub>由 ❤️ 和无数杯咖啡驱动 | 欢迎 Star ⭐ 支持我们！</sub>
</div>

---

## 🎬 配套视频教程

想更直观地学习？欢迎观看我的视频教程：

| 平台 | 链接 | 内容特色 |
|------|------|----------|
| B站 | https://space.bilibili.com/YOUR_ID | 中文讲解，适合国内用户 |
| YouTube | https://youtube.com/YOUR_CHANNEL | 中英双语字幕，面向全球 |

## 🔄 更新日志

查看 CHANGELOG.md 了解项目更新历史。

## 🙏 致谢

感谢所有为这个项目做出贡献的人！特别感谢：

- 所有传感器的开发者与制造商
- 开源社区的贡献者们
- 观看视频和提出建议的观众们

---

> 如果这个项目对你有帮助，请给它一个 ⭐ Star！这是对我们最大的鼓励！

---

这个README已经为您创建了完整的目录结构，所有二级标题都可以通过点击直接跳转到对应位置。您可以根据实际需要：

1. **修改链接**：将所有 `#` 占位符改为实际的文件路径
2. **添加内容**：在各个章节下添加具体内容
3. **更新信息**：替换联系方式和社交链接
4. **个性化**：根据您的风格调整语言和内容

需要我帮您完善某个具体章节的内容吗？