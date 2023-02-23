---
layout: post
title: Innovative-Project-Proposal
author: [Ming Lee]
category: [Lecture]
tags: [jekyll, ai]
---

This homework is to specify a Future Home application and describe the key features, list all Design Considerations and the required technologies, then draw the System Block Diagram.

---
## Test Youtube
<iframe width="1280" height="720" src="https://www.youtube.com/embed/rAP3AyPRZ_k" title="【Joeman】很貴但超美的電競螢幕！三星Odyssey OLED G8 2023開箱" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Test Picture
![](https://github.com/Ming5980/MCU-porject/blob/main/images/Perlin_noise_example.png?raw=true)
## Futre Home Applications


**Service Robots:**<br>

![](https://github.com/rkuo2000/MCU-course/blob/main/images/Future_Home_robots.png?raw=true)

---

### Homework Report
**Contents:**<br>
* **應用與功能說明**
  - Specify the future home application, and Describe the key features
  - Describe the key features which may be applied to the home space (kitchen, living room, play room, study room, bed room)
* **設計考量與所需相關技術**
  - List all design considerations and the required technologies
* **系統方塊圖**
  - Draw a System Block Diagram

---
## 機器人(未定)???
### 應用功能說明
1. 居家監控：外出時可隨時查看家裡各處狀況
2. 環境監測：溫濕度感測+瓦斯偵測+空氣品質偵測 
3. 清潔環境：撢灰塵, 除臭
4. 丟棄垃圾：丟棄小型垃圾袋至垃圾車或社區資源回收區
5. 餐飲服務：遞送調味料, 可樂, 水果, 零食

### 設計考量與相關技術
**系統設計考量：**<br>
1. 移動方式:共軸雙旋翼
2. 供電方式:電池＋自動充電
3. 聯網方式: WiFi 或 BLE to中控電腦

**所需相關技術：**
1. 飛行姿態偵測與控制: ESP32 + MPU6050 + PID controller
2. 溫濕度感測 & 氣體偵測: HTU21D + MQ2 + MQ7 + MQ135
3. 紅外線遙控: IR-LED 
4. 影像傳輸: ESP32-CAM模組
5. 物品夾具：懸吊掛勾, 磁鐵吸吊
6. 服務器: 具AI加速(GPU)
  - 影像物件偵測辨識: CSL-YOLO
  - 任務規劃控制: Mission Planner with Floorplan

### 系統方塊圖
![](https://github.com/rkuo2000/MCU-course/blob/main/images/FutureHome_flying_robot.png?raw=true)


<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*


