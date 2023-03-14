---
layout: post
title: Innovative-Project-Proposal
author: [Ming Lee]
category: [Lecture]
tags: [jekyll, ai]
---

This homework is to specify a Future Home application and describe the key features, list all Design Considerations and the required technologies, then draw the System Block Diagram.

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
## 寵物機器人
### 應用功能說明
1. 定時餵食：設定時間，在吃飯時間投放飼料
2. 供給飲水：飲水快要喝完時，適時補充水
3. 陪玩功能：能投擲、撿拾球或玩具
4. 健康檢測：當寵物狀況或行為異常時，通知飼主

### 設計考量與相關技術
**系統設計考量：**<br>
1. 移動方式:滾輪
2. 供電方式:電池＋自動充電
3. 聯網方式: WiFi 或 BLE to中控電腦
4. 垂直升降式手臂
5. 食物槽、水槽
6. 發射器

**所需相關技術：**
1. 滑軌式機器手臂 ＆ 軟式夾具
2. 影像傳輸: ESP32-CAM模組
3. 影像辨識: Jetson Nano + IMX219(攝影頭)
4. 服務器: 具AI加速(GPU)
  - 影像物件偵測辨識: CSL-YOLO
  - 任務規劃控制: Mission Planner with Floorplan

### 系統方塊圖
![](https://github.com/rkuo2000/MCU-course/blob/main/images/FutureHome_flying_robot.png?raw=true)


<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*


