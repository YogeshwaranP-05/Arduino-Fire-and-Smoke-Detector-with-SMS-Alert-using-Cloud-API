# **🔥 Fire and Smoke Alarm System with SMS Notification**

This project demonstrates how to build an advanced **Fire and Smoke Alarm System** using **Arduino**, without requiring a GSM module, to send SMS alerts. The system utilizes **WiFi connectivity** and [**Circuit Digest Cloud SMS APIs**](https://circuitdigest.com/article/free-sms-api-for-arduino-esp32-esp8266-nodemcu-raspberry-pi) to notify users about potential fire hazards in real time.

---

## **📝 Project Overview**

The Fire and Smoke Alarm System works by detecting fire or smoke through sensors connected to an **Arduino board**. Upon detection, the Arduino triggers an **alarm** and simultaneously sends an **SMS notification** to a predefined phone number using **Cloud SMS APIs**. The main components of the system are:

* **WiFi Connectivity**: Arduino connects to a **WiFi hotspot** to communicate with cloud services.  
* **Fire & Smoke Detection**: Sensors constantly monitor the environment and detect hazardous conditions.  
* **Instant Alerts**:  
  * **Buzzer Alarm** for local alerts.  
  * **SMS Notification** using HTTP requests to a cloud API.  
* **No GSM Module Required**: The system leverages **Circuit Digest Cloud SMS API** to send messages over the internet instead of using a GSM module.

This project provides hands-on experience with:

* **IoT-based sensor integration**  
* **Cloud API communication with Arduino**  
* **Wi-Fi-based data transmission**  
* **SMS alert systems**  
* **Embedded system design**

---

## **🛠 Components Required**

* **Arduino Uno R4 WiFi Dev Board** – Microcontroller for processing sensor data and WiFI handling  
* **Smoke Detector (MQ-2 / MQ-135)** – Detects smoke levels  
* **Flame Sensor** – Detects fire  
* **Buzzer** – Provides an audible alarm  
* **LED Indicator** – Alerts users visually  
* **Jumper Wires** – Electrical connections  
* **Power Supply (5V / 9V)** – Powers the Arduino and sensors

---

## **🗂 Project Structure**

/fire\_smoke\_alarm\_system  
|-- /Code                       \# Arduino sketch (.ino)  
|-- /Circuit-Diagram      \# Circuit diagram and wiring illustrations  
|-- /Block Diagram       \# System’s architecture diagram

---

## **⚙️ Installation and Setup**

### **1️⃣ Clone the Repository:**

git clone [https://github.com/YogeshwaranP-05/Arduino-Fire-and-Smoke-Detector-with-SMS-Alert-using-Cloud-API.git](https://github.com/YogeshwaranP-05/Arduino-Fire-and-Smoke-Detector-with-SMS-Alert-using-Cloud-API.git)  
cd Fire-Smoke-Alarm-System

### **2️⃣ Connect Components:**

* Start making connections from the circuit diagram  
* Attach **fire & smoke sensors** to digital input pins.  
* Connect the **buzzer and LED** to the output pins.  
* Ensure the system is powered with a **5V or 9V supply**.

### **3️⃣ Upload the Code:**

* Open **`Fire_Smoke_Detector_SMS.ino`** in the **Arduino IDE**.  
* Enter the **WiFi credentials** in the code.  
* Configure the **API endpoint** for SMS alerts.  
* Select the appropriate **board and COM port**.  
* Upload the code to **Arduino**.

### **4️⃣ Run the System:**

* Place the sensors in a test environment.  
* Introduce smoke or flame to test the system.  
* Observe the **buzzer alarm** and **SMS notification** on your phone.

---

## **📝 Code Explanation**

* **WiFi Connection**: The Arduino connects to a WiFi network using the onboard ESP32.  
* **Sensor Monitoring**: Fire and smoke sensors constantly check for hazard conditions.  
* **Triggering Alerts**:  
  * If a fire/smoke event is detected, the buzzer and LED are activated.  
  * An **HTTP request** is sent to the **Circuit Digest Cloud SMS API** with the recipient's phone number and alert message.  
* **SMS Delivery**:  
  * The cloud service receives the request and sends an SMS notification to the predefined phone number.  
  * This eliminates the need for a **GSM module** in the Arduino setup.

---

## **🤝 Contributing**

We welcome contributions\! Feel free to fork this repository, enhance the project, and submit a pull request.

---

## **🧩 License**

This project is licensed under the **GNU GPL V3.0 License**. See the LICENSE file for details.

---

## **📧 Contact**

For any queries or suggestions, visit our **Official Website**: [www.circuitdigest.com](http://www.circuitdigest.com).

For a complete tutorial, check out this guide: Fire & Smoke Alarm System with SMS Alert.

Happy coding and creating\! 🚀

