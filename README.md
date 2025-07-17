# Speech-Recognition System**

### 🔶 **Objective:**

To build a basic **speech recognition system** that allows **command-based control of electronic devices** using an **embedded board** (such as ESP32 or Arduino).

---

### 🔷 **System Overview:**

The system enables voice-activated control of devices like lights or fans. It utilizes a **mobile app for speech recognition** and an **embedded microcontroller** to process the command and switch the output device accordingly.

---

### ⚙️ **Components Used:**

| S.No. | Component                         | Description                        |
| ----- | --------------------------------- | ---------------------------------- |
| 1     | ESP32 / Arduino                   | Microcontroller board              |
| 2     | Mobile Phone                      | Voice input (Google Assistant/App) |
| 3     | Bluetooth Module (HC-05) or Wi-Fi | For wireless communication         |
| 4     | Relay Module                      | To switch high-voltage devices     |
| 5     | LED / Bulb / Fan                  | Output device                      |
| 6     | Jumper Wires, Breadboard          | For circuit connection             |
| 7     | Power Source                      | USB or 9V battery                  |

---

### 🖥️ **Working Principle:**

1. **User gives a voice command** like "Turn on light".
2. The **speech-to-text** mobile app converts it into a **text command** (e.g., "on").
3. The command is sent to the **ESP32** via **Bluetooth or Wi-Fi**.
4. ESP32 reads the command and **controls the connected device** (LED or relay).

---

### 🔌 **Connections:**

| ESP32 Pin | Connected To     |
| --------- | ---------------- |
| GPIO 2    | LED or Relay IN  |
| GND       | GND of LED/Relay |
| 5V        | Power Supply     |

---

### 📊 **Output:**

| Voice Command    | Action           | Device Output |
| ---------------- | ---------------- | ------------- |
| "Turn on light"  | ESP32 gets “on”  | LED turns ON  |
| "Turn off light" | ESP32 gets “off” | LED turns OFF |

**Observed Output:**

* Instant device control within 1 second
* Successfully received command via serial
* Accurate execution of command

---

### 📹 **Demo Summary:**

1. Speak the command on the mobile app.
2. ESP32 receives and interprets it.
3. The connected device (LED, fan, bulb) turns ON or OFF as per command.

---

### 📌 **Conclusion:**

This project demonstrates how speech recognition can be integrated with embedded systems for **smart automation applications** such as **home automation**, **assistive tech**, or **IoT-based control systems**.
