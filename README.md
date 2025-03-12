
---

# **IoT-Based Smart Pet House 🏡🐾**  

## 📌 **Project Overview**  
The **IoT-Based Smart Pet House** is a fully automated system designed to enhance pet care by integrating **automated feeding, temperature regulation, pet presence monitoring, and real-time alerts**. The system ensures a **comfortable and controlled environment** for pets while reducing manual effort for pet owners.  

---

## 🛠️ **System Components & Responsibilities**  

This project consists of **four Arduinos**, each handling a specific function:  

### **🔹 Arduino 1: Display & Alert System (Master)**  
- Controls the **LCD display**, **LEDs**, and **Buzzer**.  
- Displays system status and alerts pet owners.  
- Communicates with other Arduinos via **I2C communication**.  

### **🔹 Arduino 2: Feeding System (Slave 1)**  
- Controls a **servo motor** to dispense food.  
- Uses a **force sensor** to check if the pet has eaten.  
- Uses an **ultrasonic sensor** to monitor the food container level.  
- Sends data to **Master Arduino** to update the display and trigger alerts.  

### **🔹 Arduino 3: Cooling System (Slave 2)**  
- Uses a **DHT11 sensor** to measure temperature.  
- Activates a **fan** if the temperature exceeds a set threshold.  
- Sends temperature readings to **Master Arduino**.  

### **🔹 Arduino 4: Pet Monitoring System (Slave 3)**  
- Uses an **ultrasonic radar system** (servo + ultrasonic sensor) to detect pet presence.  
- Sends presence data to **Master Arduino**.  
- Triggers **LED and buzzer alerts** when the pet is absent.  

---

## 🏗️ **How It Works**  
1️⃣ **Pet Presence Monitoring** (Arduino 4): Detects if the pet is present and sends data to the master.  
2️⃣ **Feeding System** (Arduino 2): Dispenses food based on time, checks if the pet eats, and alerts if food is untouched.  
3️⃣ **Temperature Control** (Arduino 3): Monitors room temperature and activates cooling if needed.  
4️⃣ **Display & Alerts** (Arduino 1 - Master): Receives all data, updates the LCD, triggers LEDs, and sounds a buzzer for important alerts.  

---

## 🔄 **Communication Between Arduinos**  
- **I2C protocol** is used for communication.  
- Master Arduino requests data from each Slave and displays necessary alerts.  

---

## 🔬 **Research Gap & Solution**  

### **📌 Identified Gap**  
- Most existing IoT pet care systems **focus on one feature**, like feeding or monitoring.  
- No unified system integrates **feeding, monitoring, and temperature control**.  

### **✅ Our Solution**  
- Designed a **modular IoT system** where each functionality operates independently while communicating with a central control unit.  
- Ensures **real-time response** to pet needs, improving efficiency and automation.  

---

## 🔥 **Key Features**  
✅ **Automated Feeding** with real-time pet eating detection.  
✅ **Temperature Control** for pet comfort.  
✅ **Pet Presence Monitoring** with status updates.  
✅ **Real-time Alerts** using LCD, LEDs, and Buzzer.  
✅ **I2C Communication** for efficient data transfer.  

---

## 🏆 **Contributions**  

| **Team Member** | **Contribution** |  
|---------------|-------------|  
| **Dilaikshan MJA**  | Integrated all Arduinos via **I2C Communication**, tested & debugged overall system, implemented final logic for alerts & display. |  
| **Hanusjan**  | Developed **Master Arduino** (Display & Alerts), controlled LCD, LEDs, and buzzer. |  
| **Rashad**  | Implemented **radar-based pet presence detection** using **ultrasonic sensor and servo motor**. Assisted in **I2C communication**, programmed **alert mechanisms (LED & buzzer)**, and contributed to **testing & debugging**. |  
| **Hafas**  | Built the **Feeding System**, programmed servo motor for food dispensing, implemented food weight checking logic. |  
| **Sangeerthan**  | Developed **Cooling System**, integrated DHT11 sensor, and controlled fan operation. |  

---

## 🚀 **Simulation & Demo**  
- **TinkerCAD Simulation** demonstrates each feature in action.  
- Due to simulation limitations, some real-world functionalities may not be perfectly visualized.  

---

## 🔗 **Future Enhancements**  
🔸 **Mobile App Integration** for remote monitoring.  
🔸 **Camera Module** for real-time pet surveillance.  
🔸 *AI-Based Pet Behavior Analysis** using machine learning.  

---

## 📜 **License**  
This project is open-source and free to use for educational purposes.  

---

🚀 **Developed with Passion & Teamwork!** 💡🎯  

---

