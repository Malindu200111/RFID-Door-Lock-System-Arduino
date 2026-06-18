# RFID Door Lock System using Arduino

## 🔒 Overview

The **RFID Door Lock System** is a smart access control solution developed using **Arduino UNO** and an **RC522 RFID Reader**. The system allows access only to authorized RFID cards or tags, improving security for homes, offices, laboratories, and restricted areas.

When an authorized RFID card is scanned, the Arduino verifies the card's unique ID (UID), activates a relay module to unlock the solenoid door lock, and displays **"Access Granted"** on the LCD. If an unauthorized card is scanned, access is denied and the LCD displays **"Access Denied"**.

---

## ✨ Features

* RFID-based authentication
* Secure access control
* Automatic door locking
* LCD status display
* Relay-controlled solenoid lock
* Easy to add or change authorized RFID cards

---

## 🛠️ Components Used

* Arduino UNO
* RC522 RFID Reader
* RFID Cards/Tags
* Solenoid Door Lock
* Single Channel Relay Module
* 16×2 LCD with I2C Module
* Jumper Wires
* 12V Power Supply

---

## ⚙️ Working Principle

1. The RFID reader scans an RFID card.
2. Arduino reads the card's unique UID.
3. The UID is compared with the stored authorized UID.
4. If the UID matches:

   * LCD displays **Access Granted**
   * Relay is activated
   * Solenoid door lock unlocks
5. If the UID does not match:

   * LCD displays **Access Denied**
   * Door remains locked
6. After a few seconds, the door locks automatically.

---

## 🔌 Hardware Connections

### RC522 RFID Reader

| RFID Pin | Arduino Pin |
| -------- | ----------- |
| SDA      | D10         |
| SCK      | D13         |
| MOSI     | D11         |
| MISO     | D12         |
| RST      | D9          |
| VCC      | 3.3V        |
| GND      | GND         |

### Relay Module

| Relay Pin | Arduino Pin |
| --------- | ----------- |
| IN        | D8          |
| VCC       | 5V          |
| GND       | GND         |

### I2C LCD

| LCD Pin | Arduino Pin |
| ------- | ----------- |
| SDA     | A4          |
| SCL     | A5          |
| VCC     | 5V          |
| GND     | GND         |

---

## 💻 Software Requirements

* Arduino IDE
* MFRC522 Library
* LiquidCrystal_I2C Library
* SPI Library

---

## 🚀 Installation

1. Download or clone this repository.
2. Open the Arduino project in Arduino IDE.
3. Install the required libraries.
4. Connect the hardware according to the wiring diagram.
5. Upload the code to the Arduino UNO.
6. Scan an authorized RFID card to unlock the door.

---

## 📂 Project Structure

```text
RFID-Door-Lock-System-Arduino/
│
├── Arduino_Code/
│   └── RFID_Door_Lock.ino
│
├── Circuit_Diagram/
│   └── circuit_diagram.png
│
├── Images/
│   ├── hardware_setup.jpg
│   ├── prototype.jpg
│   ├── access_granted.jpg
│   └── access_denied.jpg
│
├── Documentation/
│   └── Project_Report.pdf
│
└── README.md
```

---

## 📸 Project Images

Add screenshots or photos of:

* Hardware Setup
* Circuit Diagram
* RFID Reader
* LCD Display
* Door Unlock Process
* Final Prototype

---

## 🎯 Applications

* Home Security
* Office Access Control
* Smart Door Lock Systems
* Laboratory Security
* Hostel Rooms
* Smart Cabinets

---

## 🚀 Future Improvements

* Fingerprint Authentication
* Face Recognition
* Mobile Application Control
* IoT Integration
* Cloud Database
* Email Notifications

---

## 👨‍💻 Author

**Malindu Kanishka**

Electrical & Electronic Engineering Undergraduate

---

## 📄 License

This project is licensed under the **MIT License**.
