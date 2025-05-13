# 🕒 Smart Attendance System using RFID, ESP8266, and Google Sheets

This is an IoT-based attendance system built using ESP8266, RFID reader, LCD, and buzzer. 
The system reads RFID cards and automatically logs attendance data with real-time timestamps (Asia/Kolkata timezone) to a Google Sheet using a custom AppScript.

## 🧠 How It Works

1. **Card Scan**: RFID tag is scanned by the MFRC522 reader.
2. **Microcontroller**: The ESP8266 reads the UID and sends it to a Google Sheets web app endpoint via HTTP.
3. **Real-Time Logging**:
   - The Apps Script logs the UID, realtime timestamp along with data logged in the rfid card
4. **User Feedback**:
   - LCD displays card status.
   - Buzzer confirms successful read or error.


## ⚙️ Hardware Used

- ESP8266 (e.g., NodeMCU)
- RFID-RC522 module
- I2C 16x2 LCD Display
- Buzzer
- RFID cards/tags
- Jumper wires

Make sure to install these libraries in Arduino IDE:

- `ESP8266WiFi`
- `MFRC522` by Miguel Balboa
- `LiquidCrystal_I2C`
- `Wire`
