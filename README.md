# PPG-BLE-Patch

# Low-power Wireless PPG–ECG BLE Patch

This project implements a **wearable patch** for physiological signal acquisition, focusing on **Photoplethysmography (PPG)** and **Electrocardiography (ECG)** with **Bluetooth Low Energy (BLE)** connectivity.  
Built around the **ADPD1080 Analog Front-End** and **STM32WB55 MCU**, it supports low-power operation from coin cells.

---

## 🔧 Hardware Overview
- **AFE:** ADPD1080 for optical biosignal acquisition  
- **MCU:** STM32WB55 for BLE streaming and processing  
- **Power:** Coin cell + boost converter for 3.3 V  
- **PCB:** 4-layer, impedance-controlled, Altium design  

### PCB Layout
![PCB Layout TOP](Images%20and%20Videos/PPGLEDside.png)
![PCB Layout Back](Images%20and%20Videos/PPGModuleSide.png)

### Assembled Board
![Assembled Board](Images%20and%20Videos/STMmodule.jpg)

---

## 💻 Firmware Overview
- **Evaluation Setup:** Initial ADPD1080 configuration  
- **Data Sampling:** Interrupt-driven acquisition with timestamps  
- **Final Firmware:** BLE data streaming to Android  
- **MATLAB Scripts:** Signal processing and visualization  

---

## 🎥 Assembly Video
![Assembly Video](Images%20and%20Videos/CompleteDesign.mp4)

---

## 📊 Results

| Raw PPG Signal + Processed | Processed PPG | BLE Transmission Test |
|----------------|--------------|-----------------------|
| ![PPG Raw](Results/Pre and Post Filtered SIgnal.png) | ![Processed](Results/result_2.png) | ![BLE Test](Results/result_3.png) |

---

## 🚀 How to Use
1. Clone this repository  
   ```bash
   git clone https://github.com/your-username/ppg-ecg-ble-patch.git
