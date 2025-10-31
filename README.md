# Envi-Rover

![Envi-Rover Screenshot](images/envi_rover.png)

## Description:
The **Envi-Rover** is a LoRa-based, long-range, remotely operated robotic system designed to monitor environmental parameters and detect obstacles in hazardous or inaccessible areas. The rover is controlled using `W`, `A`, `S`, `D` keys for movement and `X` to stop. Data from the rover is continuously received at the controller, allowing for real-time monitoring and control.

It integrates [ESP32](https://www.espressif.com/en/products/socs/esp32) with various sensors (temperature, humidity, illumination, and gas detection) and a LoRa communication module to transmit data over long distances. Users can access the data via [Blynk](https://blynk.io/) on mobile or PC.

---

## Features:

- **Remote Control:** Move the rover using `W`, `A`, `S`, `D` keys; `X` to stop.
- **Real-Time Data Monitoring:** Temperature, humidity, gas levels, and illumination are continuously monitored and transmitted.
- **Long-Range Communication:** LoRa module enables data transmission over large distances.
- **Obstacle Detection:** Ultrasonic sensor with servo rotation detects and avoids obstacles automatically.
- **Blynk Integration:** Live data is displayed on mobile or PC dashboards.
- **Deployment Ready:** Suitable for agriculture, disaster zones, industrial environments, and scientific research.

---

## Idea / Prototype:

- LoRa-based, long-range robotic system for environmental monitoring.
- Uses [ESP32 microcontroller](https://www.espressif.com/en/products/socs/esp32) with sensors:
  - DHT22 (Temperature & Humidity)
  - MQ135 (Gas Detection)
  - LDR (Illumination)
- Real-time LoRa communication enables control and monitoring in hazardous or inaccessible areas.
- Rover can be deployed in agriculture fields, disaster zones, industrial environments, and scientific research sites.

---

## Flowchart:

**Receiver Side** → **Controller Side**  

*(You can insert your actual flowchart image here)*

---

## Use Cases:

- **Agriculture:** Real-time environmental monitoring and surveys.
- **Disaster Management:** Monitoring air quality, temperature, and obstacles in dangerous areas.
- **Industrial Environments:** Detecting unsafe conditions or gas leaks remotely.
- **Smart Cities:** Integration into city-wide environmental monitoring networks.
- **Scientific Research:** Collecting field data in remote or difficult terrains.

---

## Technology Stack:

### Hardware:
- ESP32 Microcontroller
- LoRa (SX1278) Transceiver Module
- Sensors:
  - DHT22 (Temperature & Humidity)
  - MQ135 (Gas)
  - LDR (Light Detection)
- Power Supply / Battery Unit

### Software:
- Arduino IDE
- ESP32 board & LoRa modules (TX/RX)
- Sensor Libraries (DHT22, MQ135, LDR)
- Blynk for real-time data visualization
- System & display code for rover control

---

## How it Works:

- The rover continuously collects data from sensors and transmits it via LoRa to the controller.
- Users can send movement commands (`W`, `A`, `S`, `D`) to the rover, and `X` stops it.
- Ultrasonic sensor with servo rotates automatically to detect obstacles and avoid collisions.
- Blynk integration allows users to view real-time data on mobile or PC dashboards.
- Data can be accessed anytime, enabling remote monitoring even in inaccessible locations.

---

## Links:

- [ESP32](https://www.espressif.com/en/products/socs/esp32)
- [LoRa SX1278](https://www.semtech.com/products/wireless-rf/lora-transceivers)
- [Blynk](https://blynk.io/)
