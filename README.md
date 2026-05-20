# ESP32 Smart Home Lab: MQTT & Motion Detection

This repository contains the firmware and server configurations required to build a localized smart home node using an ESP32, a PIR motion sensor, ESPHome, and MQTT.

## 🛠️ Hardware Requirements
* 1x ESP32 Development Board
* 1x HC-SR501 PIR Motion Sensor
* 1x Breadboard
* Dupont Jumper Wires
* Micro-USB Data Cable

## 🔌 Wiring Diagram
| PIR Sensor Pin | ESP32 Pin | Description |
| :--- | :--- | :--- |
| **VCC** | `5V` (or `VIN`) | Provides 5V power to the sensor. |
| **GND** | `GND` | Ground connection. |
| **OUT** | `GPIO27` | Data signal line. |

## 🚀 Quick Start Guide

### 1. Flash the ESP32
1. Open the `src/esp32-motion-node.yaml` file and update the Wi-Fi and MQTT IP addresses to match your local network.
2. Connect your ESP32 to your computer via USB.
3. Open [web.esphome.io](https://web.esphome.io) in a Chrome or Edge browser.
4. Click **Connect**, select your USB port, and click **Install**.
5. Upload the modified YAML configuration.

### 2. Set Up the Local Server
If you are running the server environment locally via Docker on Windows, refer to the `server/local-server-setup.md` guide for the exact PowerShell deployment commands.
