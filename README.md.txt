## 🎮 ESP32 BLE Gamepad (12 Buttons + 2 Joysticks)

### 📌 Overview
This project turns an **ESP32** into a **Bluetooth gamepad controller** with:  
- ✅ 12 digital buttons  
- ✅ 2 analog joysticks (X/Y each)  
- ✅ Deadzone & calibration for smooth control  

The gamepad can connect to a PC, laptop, or Android device over **Bluetooth** and works like a real game controller.  

---

### 🛠️ Hardware Used
- ESP32 Dev Board  
- 12 Push Buttons  
- 2 Joysticks (PS2 type or analog thumbsticks)  
- Jumper wires & breadboard  

---

### ⚡ Circuit Connections
- **Buttons:** One side → GPIO pin, Other side → GND  
- **Joysticks:**  
  - LX → GPIO 32  
  - LY → GPIO 33  
  - RX → GPIO 34  
  - RY → GPIO 35  

⚠️ Buttons are configured with `INPUT_PULLUP`, so no external resistors are required.  

---

### 💻 Code Features
- Uses [**BleGamepad**](https://github.com/lemmingDev/ESP32-BLE-Gamepad) library  
- Maps analog joystick values to `-127 … 127`  
- Built-in **deadzone** to ignore small drifts  
- Inverts Y-axis for standard gamepad behavior  

---

### 🚀 How to Upload
1. Install **Arduino IDE** + ESP32 board package  
2. Install `BleGamepad` library from GitHub  
3. Upload the `ESP32_Gamepad.ino` sketch to ESP32  
4. Pair ESP32 with your PC/phone → It appears as **ESP32 Gamepad**  
5. Test in games or with Windows Game Controller settings  

---

### 📷 Demo / Preview
(Add images or GIFs of your project here — wiring diagram, real controller, gameplay demo)  

---

### 📜 License
This project is open-source under the **MIT License**.  
