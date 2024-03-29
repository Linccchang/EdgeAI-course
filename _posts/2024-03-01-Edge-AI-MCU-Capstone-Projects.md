---
layout: post
title: Edge-AI MCU Capstone Projects
author: [Richard Kuo]
category: [Lecture]
tags: [jekyll, ai]
---

Introduction to projects, development boards, system references, etc.

---
## Product Development Procedures: 
1. Define (Edge-AI) Product 
2. Choose Development Board
3. List Product Key Features
4. Draw Funcitonal Block Diagram
5. Create Project Schedule/Timeline
6. Prototyping / Proof-of-Concept (POC)
7. Function Verification / System Testing
8. Project Report & Summary

### [Edge-AI MCU project 協作平台](https://sites.google.com/view/ntou-rkuo2000-edgeai-project)

---
## Edge-AI Development Boards（開發板）
`Key Feature will determine what development board will be used!`<br>

Comparing some development boards:<br>
<table>
<tr><th> AMB82-mini </th><th> Kneron KL520</th><th> Jetson Orin NX </th><th> Pi-Zero 2W </th></tr>
<tr>
<td><img src="https://www.amebaiot.com/wp-content/uploads/2023/03/amb82_mini.png"></td>
<td><img src="https://www.everfocus.com/upload/catalog_m/b098f7b0f63a26477cd2cb5d08eb12c0.png"></td>
<td><img src="https://gcs.rimg.com.tw/g4/265/d35/playrobot-inc/d/4b/6e/22325013064558_792.png"></td>
<td><img src="https://www.oursteam.com.tw/upload/images/20230816_064445.png"></td>
</tr>
</table>

### AMB82-mini
`Audio recording & Video capturing + NN engine + WiFi & BLE/BT`<br>
![](https://www.amebaiot.com/wp-content/uploads/2023/03/amb82_mini.png)

[RTL8735B](https://www.amebaiot.com/en/amebapro2/): 32-bit Arm v8M, up to 500MHz, 768KB ROM, 512KB RAM, 16MB Flash (MCM embedded DDR2/DDR3L up to 128MB)
802.11 a/b/g/n WiFi 2.4GHz/5GHz, BLE 5.1, NN Engine 0.4 TOPS, Crypto Engine, Audo Codec, …

* [Ameba Arduino](https://www.amebaiot.com/en/ameba-arduino-summary/)<br>

* [Amebapro2 AMB82-mini Arduino Example Guides](https://www.amebaiot.com/en/amebapro2-amb82-mini-arduino-peripherals-examples)<br>

* [Amebapro2 AMB82-mini Arduino getting started](https://www.amebaiot.com/en/amebapro2-amb82-mini-arduino-getting-started/)<br>

---
## Capstone Projects（專題計畫）

<table>
<tr><th>Type</th><th>Applications   </th><th>Peripherals </th><th>Key Features          </th><th>required APIs/Libs</th></tr>
<tr><td>AIoT</td><td>Home Appliance</td><td>Camera      </td><td>Food Classification</td><td> imgclass </td></tr>
<tr><td>Toy</td><td>AI Pet </td><td>Camera+Mic</td><td>Emotion Detection</td><td> audioNN+ObjDet/imgclass </td></tr>
<tr><td>Education</td><td>AI Tutor</td><td>mic + TFT</td><td>Audio-to-Text</td><td>RecordMP4_HTTP_Post</td></tr>
<tr><td>Robot</td><td>Toy Car</td><td>Camera </td><td>Pothole Detection</td><td> ObjDet </td></tr>
<tr><td>Robot</td><td>Toy Car</td><td>Camera+IMU+InfraRed</td><td>Reinforcement Learning</td><td> MPU6050+VL53L0X </td></tr>
<tr><td>Robot</td><td>Home Agent</td><td>Camera+IMU</td><td> Self-Balancing </td><td> MPU6050 </td></tr>
<tr><td>Drone</td><td>Quadcopter</td><td>Camera+IMU</td><td> Fly-control </td><td> MPU9250+BMP280 </td></tr>
<tr><td>GenAI</td><td>Portable ChatGPT</td><td>camera/mic + TFT</td><td>Audio/Image</td><td>CaptureJpeg_HTTP_Post_JpgTxt</td></tr>
<tr><td>GenAI</td><td>Wearable ChatGPT</td><td>camera/mic + TFT</td><td>Audio/Image/Gesture/Touch</td><td> Multimodal </td></tr>
</table>

**API status:**<br>
* imgclass : Verifying
* AudioNN+ObjDet : TO-BE-VERIFIED
* RecordMP4_HTTP_Post.ino : Verified (with Ameba_whipser_server.py)
* CaptureJpeg_HTTP_Post_JpgTxt.ino : TO-BE-DEVELOPED
* VL53L0VX_IR_ranger.ino : TO-BE-DEVELOPED
* MPU6050_DMP6.ino : Verified
* MPU9250_DMP6.ino : TO-BE-DEVELOPED
* BMP280_barometer.ino : TO-BE-DEVELOPED
* ILI9341 2.4" TFT : To-be-verified
* ST7789  1.3" TFT : TO-BE-DEVELOPED 

---
### Vehicles for Modification （改裝載具）
<table>
<tr>
<td><img src="https://cdn1.techbang.com/system/excerpt_images/113469/post_inpage/57a929bbe81c765717cb2d373d197784.jpg?1709099479"></td>
<td><img src="https://mm.digikey.com/Volume0/opasdata/d220001/medias/images/2869/MFG_ESP32-S3-BOX.jpg"></td>
<td><img src="https://a.rimg.com.tw/e1/ebay/2e0/56a/devkits%40ebay/9/d3/58/3771c98e0b7103dfaff026bb9f582e25_30222264519512.jpg"></td>
</tr>
<tr>
<td><img src="https://a.rimg.com.tw/e1/ebay/c03/f47/agent0029346%40ebay/f/ce/0a/54dfde3ef38febef5598e670c1278f17_30221118817802.jpg"></td>
<td><img src="https://down-tw.img.susercontent.com/file/5a25f3ff18bfb194c3bb1ec786431a73"></td>
<td><img src="https://img.pchome.com.tw/cs/items/DEASMYA900FN51P/000001_1665724453.jpg"></td>
</tr>
<tr>
<td><img src="https://gcs.rimg.com.tw/g4/e40/afa/jif9j8j8/f/3d/2a/22347200521514_469.jpg"></td>
<td><img src="https://gcs.rimg.com.tw/g5/cad/e0b/davidhadson493/f/43/3d/22347198425917_866.jpg"></td>
<td><img src="https://github.com/rkuo2000/Robotics/blob/main/images/Vacuum_Robot.jpg?raw=true"></td>
<td><img src="https://github.com/rkuo2000/EdgeAI-course/blob/main/images/ESP32_RoboCar.jpg?raw=true"></td>
</tr>
<tr>
<td><img src="https://github.com/rkuo2000/EdgeAI-course/blob/main/images/Self-Balancing-Car.jpeg?raw=true"></td>
<td><img src="https://s.yimg.com/zp/images/6192E5630B431848DEE2F7C96305532D6F700286"></td>
<td><img src="https://proguideah.com/wp-content/uploads/2024/01/LG-smart-home-AI-agent-CES-2024.jpg"></td>
<td><img src="https://www.thefunaticsblog.com/wp-content/uploads/2023/10/Screenshot-2023-10-09-090123-1024x597.jpg"></td>
</tr>
<tr>
<td><img src="https://gcs.rimg.com.tw/g2/2/97/4e/21606776067918_370.jpg"></td>
<td><img src="https://gcs.rimg.com.tw/g2/8/44/64/21651860715620_880.jpg"></td>
<td><img src="https://gcs.rimg.com.tw/g1/5/53/3f/21746333748031_651.jpg"></td>
<td><img src="https://gcs.rimg.com.tw/g1/8/67/0d/22251865967373_876.jpg"></td>

</tr>
</table>

---
### Components 
* [日本 IWAYA 拉拉散步狗](https://www.ruten.com.tw/item/show?21713666818852)
![](https://gcs.rimg.com.tw/g2/f/37/24/21713666818852_267.jpg)
* [越野遙控車](https://www.ruten.com.tw/item/show?22347200521514)
![](https://gcs.rimg.com.tw/g4/e40/afa/jif9j8j8/f/3d/2a/22347200521514_469.jpg)
* [四驅遙控越野汽車](https://www.ruten.com.tw/item/show?22139378684238)
![](https://gcs.rimg.com.tw/g9/3c3/78b/ff742155456/d/4e/22139378684238_637.jpg)
* [水陸兩棲遙控船汽車](https://www.ruten.com.tw/item/show?22347198425917)
![](https://gcs.rimg.com.tw/g5/cad/e0b/davidhadson493/f/43/3d/22347198425917_866.jpg)
* [QAV250 穿越機 套餐 套件](https://www.ruten.com.tw/item/show?21606776067918)
![](https://gcs.rimg.com.tw/g2/2/97/4e/21606776067918_533.jpg)
* [變形陸空兩用遙控無人機航拍](https://www.ruten.com.tw/item/show?22251865967373)
![](https://gcs.rimg.com.tw/g1/8/67/0d/22251865967373_876.jpg)
* [S91折疊無人機 自動避障航拍機](https://www.ruten.com.tw/item/show?22009310684959)
![](https://gcs.rimg.com.tw/g0/e60/66e/chengyi008/5/c7/1f/22009310684959_870.jpg)
* [Parrot Swing 速影 直升翼 滑翔/四軸兩用機](https://www.ruten.com.tw/item/show?22329258033212)
![](https://gcs.rimg.com.tw/g2/2/60/3c/22329258033212_320.jpg)
* [2自由度機械手臂夾爪子](https://www.ruten.com.tw/item/show?22339800651177)
![](https://gcs.rimg.com.tw/g5/a96/4e3/a0918379379/a/11/a9/22339800651177_202.jpg)
* [機器人微型電動仿生柔性手爪金屬夾持器](https://www.ruten.com.tw/item/show?22343001464997)
![](https://gcs.rimg.com.tw/g5/41c/c6a/ssam82410/6/b8/a5/22343001464997_757.jpg)
* [智能平衡車](https://shopee.tw/%E5%85%8D%E9%81%8B-%E6%99%BA%E8%83%BD%E5%B9%B3%E8%A1%A1%E8%BB%8A-%E6%88%90%E4%BA%BA%E4%BB%A3%E6%AD%A5%E8%BB%8A-%E9%9B%BB%E5%8B%95%E6%BB%91%E6%9D%BF%E8%BB%8A-%E9%9B%99%E8%BC%AA%E5%B9%B3%E8%A1%A1%E8%BB%8A-110V%E5%85%92%E7%AB%A5%E5%B9%B3%E8%A1%A1%E8%BB%8A-%E9%80%9A%E7%94%A8%E5%B9%B3%E8%A1%A1%E8%BB%8A-%E5%B8%B6%E6%89%B6%E6%A1%BF%E5%85%A9%E8%BC%AA%E4%BB%A3%E6%AD%A5%E8%BB%8AK10892-i.691046991.23539136949)
![](https://down-tw.img.susercontent.com/file/tw-11134201-7r98o-lkqh27uefic512)
* [小米九號平衡車Plus](https://www.ruten.com.tw/item/show?21726606095037)<br>
![](https://gcs.rimg.com.tw/g1/1/02/bd/21726606095037_310.jpg)

---
## System References （系統參考）
### AI 巧虎
![](https://cdn1.techbang.com/system/excerpt_images/113469/post_inpage/57a929bbe81c765717cb2d373d197784.jpg?1709099479)
<iframe width="720" height="405" src="https://www.youtube.com/embed/FyZ7BbS0ksE" title="〈こどもちゃれんじほっぷ〉 AI「しまじろう」のご紹介" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
### [ESP32-S3-Box](https://www.espressif.com/en/news/ESP32-S3-BOX_video) 
[Unleashing the Power of OpenAI and ESP-BOX](https://blog.espressif.com/unleashing-the-power-of-openai-and-esp-box-a-guide-to-fusing-chatgpt-with-espressif-socs-fba0b2d2c4f2)<br>
* [貿澤電子](https://www.mouser.tw/ProductDetail/Espressif-Systems/ESP32-S3-BOX-3?qs=sGAEpiMZZMuqBwn8WqcFUipNgoezRlc4u4gjCc9cblNcfZiByE2ecw%3D%3D)
![](https://hackster.imgix.net/uploads/attachments/1625815/esp32-s3-box-3_cover_GSYrNNltxp.jpg?auto=compress%2Cformat&w=830&h=466.875&fit=min&dpr=1)

---
### ChatGPT SmartWatch
<iframe width="1273" height="716" src="https://www.youtube.com/embed/ZCVDDcTL8xQ" title="World&#39;s First ChatGPT AI Smartwatch" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
### AI Pin
<iframe width="1273" height="716" src="https://www.youtube.com/embed/JA1CGnsKrSE" title="AI Pin 最新的AI科技有多蠢！？" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
### [Rabbit R1](https://www.rabbit.tech/)
<iframe width="1042" height="586" src="https://www.youtube.com/embed/Hy2r7luwS10" title="First Look at Rabbit R1 AI Device" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
### 小米9號平衡車PLUS 
<iframe width="1273" height="716" src="https://www.youtube.com/embed/gFt0NosqWNM" title="『新品Talk』(下集)小米9號平衡車PLUS性能實測竟然有BUG?小米9號1、2代大PK[黃小潔Jerry]" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
### LG Smart Home AI Agent
<iframe width="452" height="804" src="https://www.youtube.com/embed/XPYzX5A6pt4" title="LG’s latest robot wants to run your home for you. #CES2024 #Technology" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
### Disney's Bipedal Robot (BD-1)
<iframe width="886" height="498" src="https://www.youtube.com/embed/-cfIm06tcfA" title="A New Approach to Disney’s Robotic Character Pipeline" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
### Disney's Judy Hopps 
<iframe width="886" height="498" src="https://www.youtube.com/embed/XEp3OV9k_O4" title="Disney Imagineers Demo New Relatable Robotic Character" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
### Top 10 best personal robots you can buy in 2024
<iframe width="1036" height="583" src="https://www.youtube.com/embed/FfELSE0Dh20" title="Top 10 best personal robots you can buy in 2024." frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
### Humanoid Robot
<iframe width="999" height="562" src="https://www.youtube.com/embed/tpp8cykrauk" title="圖 01 OpenAI + 微軟的人工智能機器人更新令科技界震驚" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<iframe width="853" height="480" src="https://www.youtube.com/embed/bH1XzArE9rM" title="新型開普勒人工智能機器人（帶 40 個軸，展示多項新一代功能，價格揭曉)" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*


