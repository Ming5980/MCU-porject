---
layout: post
title: MCU Capstone Projects
author: [Richard Kuo]
category: [Lecture]
tags: [jekyll, ai]
---

MCU 專題實作: 溫溼度物聯網裝置, 藍牙3D滑鼠, 藍牙遙控自走車, 兩輪自平衡小車, 迷你四軸無人機, ROS2遙控機器人

---
## 溫溼度物聯網裝置
![](https://github.com/rkuo2000/MCU-course/blob/main/images/Example_DHT11.jpg?raw=true)

### [io.adafruit.com](https://io.adafruit.com/)
註冊帳號以取得金鑰
![](https://d2794n4cyhr13z.cloudfront.net/packs/production/media/src/images/landing/dashboard-chart-9f23396336bf1e7a3269416264d36544.png)

### Examples> ESP32 > ESP32_adafruitio_DHT11
範例程式中修改AIO_Name(帳號名稱) 及 AIO_KEY(金鑰)<br>

ESP32燒錄程式後，連線WiFi, ESP32會讀取DHT11溫濕度, 上傳至你的io.adafruit.com帳號中<br>

[ESP32_adafruitio_DHT11.ino](https://github.com/rkuo2000/Arduino/blob/master/examples/ESP32/ESP32_adafruitio_DHT11/ESP32_adafruitio_DHT11.ino)<br>

---
## 藍牙3D滑鼠
![](https://github.com/rkuo2000/MCU-course/blob/main/images/Example_ESP32_MPU6050.jpg?raw=true)

### Arduino Library> ESP32 BLE mouse
[ESP32 BLE Mouse Library](https://github.com/T-vK/ESP32-BLE-Mouse)<br>

---
### Examples> ESP32 BLE mouse> MouseButton
![](https://github.com/rkuo2000/MCU-course/blob/main/images/Examples_ESP32_BLE_mouse_MouseButton.png?raw=true)

---
### Sketch>ESP32_BLEmouse_MPU6050.ino
ESP32燒錄程式後，連線具有藍牙之個人電腦, ESP32+MPU6050即可成為3D滑鼠<br>

[ESP32_BLEmouse_MPU6050.ino](https://github.com/rkuo2000/arduino/blob/master/examples/ESP32/ESP32_BLEmouse_MPU6050/ESP32_BLEmouse_MPU6050.ino)<br>
![](https://github.com/rkuo2000/MCU-course/blob/main/images/Sketch_ESP32_BLEmouse_MPU6050.png?raw=true)
![](https://github.com/rkuo2000/MCU-course/blob/main/images/Sketch_ESP32_BLEmouse_MPU6050_monitor.png?raw=true)

---
## 藍牙遙控自走車
![](https://github.com/rkuo2000/MCU-course/blob/main/images/ESP32_RoboCar.jpg?raw=true)

### 藍牙遙控App
[http://ai2.appinventor.mit.edu/](http://ai2.appinventor.mit.edu/)<br>
[手機App開發平台使用介紹](https://rkuo2000.github.io/MCU-course/lecture/2022/04/23/MIT-App-Inventor-2.html)<br>

### App程式範例: [BT2RC.aia](https://github.com/rkuo2000/MCU-course/blob/main/files/BT2RC.aia)
![](https://github.com/rkuo2000/MCU-course/blob/main/images/AppInventor2_BT2RC_Designer.png?raw=true)
![](https://github.com/rkuo2000/MCU-course/blob/main/images/AppInventor2_BT2RC_Blocks.png?raw=true)

---
### [RoboCar程式範例](https://github.com/rkuo2000/Arduino/tree/master/examples/Robots/RoboCar) 
[ESP32_RoboCar_TB6612_MPU6050_SR04_BLE](https://github.com/rkuo2000/Arduino/tree/master/examples/Robots/RoboCar/ESP32_RoboCar_TB6612_MPU6050_SR04_BLE)<br>

---
## 兩輪自平衡小車
![](https://github.com/rkuo2000/MCU-course/blob/main/images/ESP32_SelfBalance_RoboCar.png?raw=true)

### Examples> Robot > TwoWheelSelfBalance
[TwoWheelSelfBalance.ino](https://github.com/rkuo2000/Arduino/blob/master/examples/Robots/TwoWheelSelfBalance/TwoWheelSelfBalance.ino)

---
## 迷你四軸無人機
![](https://github.com/rkuo2000/MCU-course/blob/main/images/ESP32_miniCopter.jpg?raw=true)

### ESP32Copter
[ESP32Copter程式範例](https://github.com/rkuo2000/Arduino/tree/master/examples/Robots/Esp32Copter)<br>

---
## ROS2遙控機器人
[ROS2介紹與安裝](https://rkuo2000.github.io/Robotics/lecture/2022/07/30/Robot-Operating-System.html)<br>
[microROS介紹與安裝](https://rkuo2000.github.io/Robotics/lecture/2022/07/31/microROS.html)<br>

### ROS2遠程遙控器
[如何使用esp32從零製作一個ROS2的teleop遙控器](https://chowdera.com/2021/10/20211023102532530v.html)

### Sketch> ESP32 > ESP32_ADC_Joystick
![](https://github.com/rkuo2000/MCU-course/blob/main/images/Example_ESP32_ADC_Joystick.jpg?raw=true)

[ESP32_ADC_Joystick.ino](https://github.com/rkuo2000/Arduino/blob/master/examples/ESP32/ESP32_ADC_Joystick/ESP32_ADC_Joystick.ino)<br>
![](https://github.com/rkuo2000/MCU-course/blob/main/images/Sketch_ESP32_ADC_Joystick.png?raw=true)

[ESP32_ROS2_Teleop.ino]()

---
### ROS2 Turtlesim
<img width="50%" height="50%" src="https://github.com/rkuo2000/Robotics/blob/main/images/ros2_run_turtlesim.png?raw=true">
On Ubuntu22.04, run ROS2 (humble)<br>
* ROS2 turtlesim
```
source_ros2
ros2 run turtlesim turtlesim_node
```

* ROS2 node & topic
```
source_ros2
ros2 node list
ros2 node info /turtlesim
ros2 topic echo /turtle1/cmd_vel
```
* ROS2 teleop_key
```
source_ros2
ros2 run turtlesim turtle_teleop_key
```

---
### ROS2遙控機器人
[ROS2_ESP32Bot](https://github.com/shirokunet/ros2_esp32bot)<br>
![](https://lh3.googleusercontent.com/x5sKEv_RQhGm5qCC-zDFmF9Mf-7K5WzPjpGSWVuvPcdpRqZMKhRcK4JSG6n6v8DPT4hlyWjmBaCpWVXGSWsfrTU7P2oyu0X9WnevnFgQllUyaeGwhWExFSdQxrCVoln-JorZiDvM0A)

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*


