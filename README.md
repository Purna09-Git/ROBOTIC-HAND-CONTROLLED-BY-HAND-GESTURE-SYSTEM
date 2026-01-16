# **Robotic Hand Controlled by Hand Gestures**

## **Project Overview**
This project features an **Arduino-based robotic hand** designed to mimic human hand movements in real-time. By using a specialized glove equipped with **flex sensors**, the system captures the nuances of finger gestures and translates them into precise robotic actions.

This interface bridges the gap between the physical human world and digital robotics, offering a natural and intuitive mode of interaction. It is designed for precision handling in environments where direct human contact may be unsafe.

---

## **Key Features**
* **Gesture Recognition:** Uses flex sensors to record meaningful finger movements.
* **Proportional Control:** Arduino processes voltage changes to trigger servos to move a proportional amount.
* **Wired Transmission:** Reliable data transfer from the glove to the microcontroller.
* **Precision Handling:** Capable of mimicking routine human hand functions.

<img width="555" height="388" alt="Project Setup" src="https://github.com/user-attachments/assets/d2d92c39-0f12-4c32-9ac1-2ef9df356c66" />

---

## **🛠 Methodology & Components**
The system operates on the principle of **voltage division**. As the flex sensors bend, their resistance changes; the Arduino measures this change through its analog input pins.

<img width="559" height="330" alt="Circuit Schematic" src="https://github.com/user-attachments/assets/56133e40-ee70-4eb9-9873-042a4f780b64" />



### **Hardware Components**
* **Microcontroller:** Arduino (The "brain" of the project).
* **Sensors:** 5x Flex Sensors (acting as variable resistors).
* **Actuators:** 5x Servo Motors (to physically move the fingers).
* **Power Supply:** 9V Battery.
* **Circuitry:** 22kΩ static resistors for voltage divider circuits.

---

## **⚙️ How It Works**
1.  **Sensing:** Flex sensors are mounted on a glove. When a finger bends, the resistance of the sensor changes proportionally.
2.  **Processing:** This resistance change is converted into a voltage change. The Arduino reads this via its **Analog Input Pins**.
3.  **Action:** The Arduino processes these inputs and generates **PWM signals**, triggering the servos to move the robotic fingers to the corresponding angle.

---

## **🔧 Assembly Instructions**

### **Circuitry & Wiring**
* **Grounding:** Connect the **main GND wire** to all individual ground wires from the sensors before plugging it into the Arduino’s GND pin.
* **Analog Input:** Each sensor's signal wire must be plugged into a separate analog input pin.
* **Color Coding:** Use **Red** for positive voltage and **Black** for ground connections for easier troubleshooting.
