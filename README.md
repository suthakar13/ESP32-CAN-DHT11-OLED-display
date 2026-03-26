# ESP32-CAN-DHT11-OLED-display
ESP32 CAN Communication with DHT11 and OLED
## 📌 Overview
This project demonstrates CAN communication between two ESP32 boards using MCP2515 modules.

- Sender: Reads temperature & humidity from DHT11 and sends via CAN
- Receiver: Displays data on OLED and sends ACK

## 🛠️ Hardware Used
- ESP32 (2 units)
- MCP2515 CAN Module (2 units)
- DHT11 Sensor
- OLED Display (SSD1306)
- Connecting wires

## 🔌 Wiring

### MCP2515 ↔ ESP32
- CS → GPIO 5  
- SCK → GPIO 18  
- MOSI → GPIO 23  
- MISO → GPIO 19  
- VCC → 5V  
- GND → GND  

### OLED ↔ ESP32
- SDA → GPIO 21  
- SCL → GPIO 22  

### CAN Bus
- CANH ↔ CANH  
- CANL ↔ CANL  
- GND ↔ GND  

## ⚙️ Features
- CAN communication (500 kbps)
- Temperature & Humidity transmission
- OLED display output
- ACK mechanism for reliability

## ▶️ How to Run
1. Upload sender code to ESP32 #1  
2. Upload receiver code to ESP32 #2  
3. Connect CAN wires (CANH, CANL, GND)  
4. Open Serial Monitor (115200 baud)  

## 📸 Output
- Serial Monitor shows transmitted/received data  
- OLED displays temperature & humidity  

## 🚀 Future Improvements
- Add WiFi dashboard  
- Data logging  
- Multiple node CAN network  

## 👨‍💻 Author
suthakar
<img width="1024" height="1024" alt="CAN" src="https://github.com/user-attachments/assets/f6bef5d6-d292-46db-bfdf-1b7eb9635936" />



