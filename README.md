# 🚀 Joystick-Controlled Maqueen V2 Plus

## 🔥 Overview

Welcome to the **ultimate** way to control your **Maqueen V2 Plus** robotic car! 🎉  
This **Android app** lets you seamlessly **drive** the Maqueen using a **virtual joystick**! 🚗💨  
The joystick transmits movement commands over **WiFi** to an **ESP8266 module**, which then directs the Maqueen’s motors with precision.  

---

## ⚡ Key Features

✅ **Fluid Joystick Navigation** – Move effortlessly in **8 directions** 🔄  
✅ **Real-Time Feedback** – Monitor **X, Y coordinates, angle, & distance** 📊  
✅ **Wireless Control via HTTP** – Commands sent to the **ESP8266** 📡  
✅ **Animated Joystick Movements** – Watch the virtual joystick in action 🎥  
✅ **Customizable UI** – Adjust joystick **size, transparency & sensitivity** 🎨  

---

## 🎮 How It Works  

### 🕹️ Joystick Interaction  

- The **virtual joystick** captures your touch and **calculates movement direction**.  
- It maps your input to **8 directions**, ensuring **precise** and **responsive** control.  

### 🔄 Real-Time Movement Feedback  

- As you **drag the joystick**, the UI **dynamically updates** X, Y positions, angle, and movement distance.  

### 📡 Sending Commands to the Maqueen  

Each joystick movement is converted into an **HTTP request** like:  

```java
String esp8266Ip = "http://192.168.4.2";  // Replace with your ESP8266 IP  
String direction = "forward";  
String requestUrl = esp8266Ip + "/" + direction;  
sendHttpRequest(requestUrl);  
```

- The **ESP8266 interprets these commands** and **activates the Maqueen’s motors** accordingly. 🚀  

### 🎥 Animated Joystick Movements  

- A **graphical ball** moves in sync with your input, making interactions feel natural! 🏀  

---

## 🛠️ Installation & Setup  

### 📲 Install the Android App  

1️⃣ Download & install the APK.  
2️⃣ Connect your phone to the **same WiFi network** as the ESP8266.  

### 🔌 Set Up ESP8266 & Maqueen  

1️⃣ Configure the **ESP8266** to connect to WiFi.  
2️⃣ Wire the Maqueen’s **motors** to the ESP8266’s **GPIO pins**.  
3️⃣ Set up a **lightweight HTTP server** on the ESP8266 to handle movement requests.  

---

## ⚡ Upload Code to the Maqueen  

The **Maqueen V2 Plus** runs on a **micro:bit** that executes custom code.  
Use the following link to access the micro:bit code and upload it to your Maqueen:  

🔗 **[Maqueen micro:bit Code](https://makecode.microbit.org/_i45P0oazKhjE)**  

Look of the **Maqueen** first-hand:
![20250319_114806](https://github.com/user-attachments/assets/dbfbd373-54d6-49ab-9619-1c01b0b2c285)


---

## 🚀 Run the App & Start Driving!  

✅ Open the app.  
✅ Move the joystick.  
✅ Watch your **Maqueen zoom around!** 🚗💨  

---

## 📸 Joystick Interface Preview  

![joy](https://github.com/user-attachments/assets/812493e7-3b21-4228-a4ab-1e0ec2a27f09)


---

## 🚀 Future Upgrades  

🔹 **Bluetooth Mode** – Control without WiFi! 📶  
🔹 **Adjustable Speed & Sensitivity** – Fine-tune your driving experience ⚙️  
🔹 **Voice Control** – Give voice commands to steer the Maqueen! 🎙️  
🔹 **Obstacle Detection** – Smart sensors to avoid collisions! 🚧  

---

## 🤝 Want to Contribute?  

💡 Have ideas to improve the app? **Fork this project & contribute!**  

---

Now go ahead, take the wheel, and enjoy the thrill of joystick-controlled robotics! 🏎️✨  

