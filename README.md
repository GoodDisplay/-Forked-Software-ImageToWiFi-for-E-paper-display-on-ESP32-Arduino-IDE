# ![image](https://user-images.githubusercontent.com/57305534/200108501-c3dd7f1d-065d-409b-84b0-900c6815509e.png)Good-Display-ImageToWiFi

[See the original product page for more info](https://www.good-display.com/product/438.html) 
<br/>

Product Gallery for the 12.48 inch E-paper module-GDP1248RW1
------------------------------------------------------------------------------------------------------------
<img src="https://www.good-display.com/repository/image/5c221e38-e74e-4146-86fe-3836e185e16d.jpg_640xaf.jpg" />
<br/>

<img src="https://www.good-display.com/repository/image/e60bf3ec-47cf-4f08-9e75-722ddb4c96c5.jpg_640xaf.jpg" />
<br/>

<img src="https://www.good-display.com/repository/image/cb58d72a-b3ab-4227-9ac0-606e9bf34405.jpg_640xaf.jpg" />
<br/>



[![image](https://user-images.githubusercontent.com/57305534/200110058-42a41f14-0e68-4ae3-abe2-8b9c715a4117.png)Direct Purchase Gateway](https://buy-lcd.com/products/1248-inch-large-e-ink-display-uc8179-big-epaper-color-screen-gdey1248z51) 
<br/>
------------------------------------------------------------------------------------------------------------

# ⚙️Software Description


This software enables users to use WiFi from ESP32-S on Arduino IDE to drive the 7.5 inch and 12.48 inch E-paper displays with B/W color and also B/W/R color to maker a very beautiful, aesthetic digital signage device!<br/>

Via ImageToWiFi, multiple devices can be supported for easy managment online, which users can deploy with zero extra cost for small-size application scenarios like home use, small supermarkets, smart office etc. Good Display has already offered you with this easy and helpful E-paper display solution!!!
Please feel free to get your hands on it!

<br/>

<br/>

# ⚙️软件简介


ImageToWiFi上位机软件使用户能够在Arduino IDE上使用ESP32-S的WiFi来驱动7.5英寸和12.48英寸的电子纸显示器（支持黑白单色以及黑白红三色的屏幕），您可以选择用我们提供的外壳或者您自己制作的，最后可以得到一个漂亮、美观的电子显示标牌！<br/>

ImageToWiFi支持多个设备同时在线管理，用户在此基础上可以零成本部署多个墨水屏设备，用于家庭个人使用、小型超市、智能办公等小型应用场景。Good Display已经为您提供了这种简单而高效的的电子纸显示屏解决方案！！！强烈恳请您立即尝试！！！

<br/>

<br/>

# ⚙️Instruction

- [See the user manual online](https://www.good-display.com/companyfile/890.html) 
<br/>

1. Software Preview
<br/>
<img src="https://www.good-display.com/repository/image/88862c48-637b-46f5-a780-83dcc0662501.jpg" />
<br/>
2. Device Network Setting
<br/>
2.1 Query Local IP Address
<br/>
<img src="https://www.good-display.com/repository/image/c8f59a2a-3482-4aad-ac54-f48a060053cc.jpg" />
<br/>
Open ImageToWiFi software, and the status bar will automatically retrieve the IP address of the current computer. Through this, you can know the current network segment. The IP address in the following figure is 192.168.5.7, and the network segment is '5' (this network segment will be used when setting the device WiFi). Change the network segment in the software to 5. Display local computer IP address:
<br/>

Set current network segment
<br/>
<img src="https://www.good-display.com/repository/image/ebdd98ba-98b0-4ed4-8f51-fe3bee6553a1.jpg" />
<br/>

2.2 Install Arduino Program Editing Software
<br/>
This development board adopts serial port to download programs, which requires Arduino programming software, type-C cable, CH340 driver and esp32_package_v1_0_2 firmware package and python-2.7.17 plug-in.

The operation steps are as follows:
<br/>
1) For the first download, install CH340 driver and ESP32 on the computer_package_v1_0_2 firmware package, python-2.7.17 plug-in.
<br/>
2) Firmware package: esp32_package_v1_0_2. The unzipped file name is espressif. Unzip the espressif folder and put it in the arduino/hardware directory. During installation, the Arduino programming software must be closed, and the firmware package can also be searched directly in the Arduino library manager.
<br/>
3)Use the default installation path for CH340 driver and python-2.7.17 plug-in.
<br/>
4) Run the program file get.exe in esp32/tools(you must have installed the python plug-in).

<br/>
<img src="https://www.good-display.com/repository/image/d4a63e46-9365-4a99-9169-e457ffe1b0c6.jpg" />
<br/>

5) Connect the Type-C interface of the development board to the computer with USB cable.
<br/>
6) Open Arduino.ino engineering document in the driver folder with Arduino 1.8.6.

<br/>
<img src="https://www.good-display.com/repository/image/46a0ca16-5c3f-4c2c-bcf9-e6ffb69dc072.jpg" />
<br/>


7) Set in 'tools'

Click position 1 to select the development board model'WEMOS LOLIN32'

Click position 2 to select serial port baud rate '115200'

Click position 3 to select COM port.

Click position 4 to select the programmer model, and here select'AVRISP mkII'

Click position 5  to compile the program

Click position 6  to download the program to the development board.

After the downloading, first power off the development board, connect the electronic paper display screen to the adapter board, and then power on again so that E-paper can display normally.

Note: if the compiler prgmpts 'invalid library found' during program compilation, please ignore this prompt, which will not affect the actual program download.

<br/>

<img src="https://www.good-display.com/repository/image/6eb59e36-5182-4ee7-8675-405c944c0be4.jpg" />
<br/>

2.3 Device WiFi Setting 

The customer needs to put the WiFi user name, password, network segment and IP number, of which the network segment '' is the field automatically identified by imagetowifi above, and the IP number range is 201~210. Different device numbers cannot be repeated. At present, up to 10 groups of devices are supported to be online at the same time. After setting the parameters, download the program to the corresponding device according to the above down steps.
<br/>

<img src="https://www.good-display.com/repository/image/c1e93114-8808-4df2-9951-97d07e0428b9.jpg" />
<br/>


3. Image Import   

Image import: click the "Open File" button, select the created image, and note that the color and resolution of the image should correspond to the current device. After the image is imported, the software will prompt the size, resolution, color and other parameters of the image to be displayed.
 
<br/>

<img src="https://www.good-display.com/repository/image/666dbffa-1a21-4820-b62b-3caa1a03a672.jpg" />
<br/>


4. Device Connection

Power the device. Generally, it is recommended that the power supply is above 5v2a. Open ImageToWiFi software, and the status bar will automatically query the current online status of the device. When the status indicator turns green, it means that the device of the corresponding network segment has been successfully online.

<br/>

<img src="https://www.good-display.com/repository/image/5f7248c7-8b0f-47e4-a89f-d0e9050e81e6.jpg" />
<br/>


5. Data Transmission

Select the IP number to be sent and click "connect". When the data transmission is normal, the left information bar will display the current data transmission progress. When the data transmission is completed, the software will display "Data send is OK!"

<br/>

<img src="https://www.good-display.com/repository/image/de982230-89ac-4232-a38b-411e575d28f8.jpg" />
<br/>



# SPECIAL OFFER FOR OUR PRODUCTS!<img src="https://img.alicdn.com/tfs/TB1OQux3hD1gK0jSZFsXXbldVXa-134-32.png" /> 
- [Direct Link for AliExpress Online Store](https://goodisplay.aliexpress.com/store/top-rated-products/1100401572.html?spm=a2g0o.store_pc_topSellerIng.8148362.6.3b122f6c9QvdHT&origin=n&SortType=orders_desc) 
<br/>Welcome to order products on AliExpress!!! Very good bargain!

<br/>

# BUYEPAPER ONLINE SHOP IS ALSO NICE CHOICE
- [Direct Link](https://www.buy-lcd.com/collections/special-offer) 
<br/>Send inquiry to us!!
![image](https://user-images.githubusercontent.com/57305534/209752673-fc672971-5e79-4a46-8b65-dd5edb4bc92d.png)


<br/>

# YOU MIGHT FIND SOME SURPRISE HERE ON OZ ROBOTICS<img src="https://ozrobotics.com/wp-content/uploads/2019/10/OzRobotics-2019.png" /> 
- [Direct Link for OZ ROBOTICS](https://ozrobotics.com/vendors/gooddisplay/) 

<br/>
<br/>


