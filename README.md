# Hi, I'm Manideep Reddy Vangala 👋

<p align="left">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&pause=1000&color=2496ED&width=500&lines=Programming+ESP32+%26+Microcontrollers;Building+Motorsport+Telemetry;Designing+Wearable+Health+Tech" alt="Typing SVG" />
  </a>
</p>

---

### 💻 About Me & Professional Profile

I am an **Embedded Systems Engineer** specializing in high-performance C/C++ development, real-time operating systems (RTOS) architectures, and low-latency hardware telemetry. I am passionate about bridging the gap between physical sensors and cloud-based analytics to build reliable, power-efficient smart systems.

- 💡 **My Philosophy:** Writing clean, non-blocking, and power-optimized code to ensure robust hardware-software integration for real-world reliability.
- 🎓 **Core Interests:** IoT Architectures, Edge AI/ML, Wearable Biomedical Devices, High-Speed Telemetry, and Intelligent Systems.
- 🤝 **Collaboration:** Open to collaborating on innovative IoT projects, medical wearable technologies, and firmware engineering roles.

---

### ⚡ Currently Working On

#### 🩺 ESP32 Brachial Health Monitoring System
A multi-sensor wearable diagnostic band designed for non-invasive, continuous brachial artery health and vitals monitoring.

- **The Objective:** Real-time physiological telemetry (Heart Rate, SpO2, Skin/Body Temperature) optimized for continuous wear.
- **Hardware Integration:**
  - **ESP32** dual-core processor managing multi-threaded sensor reading task queues.
  - **MAX30102** Pulse Oximeter & Heart-Rate Sensor for PPG readings.
  - **MLX90614** Contactless Infrared Thermometer for body/skin temperature logging.
  - **BMP280** Barometric Pressure & Ambient Temperature Sensor.
  - **ADXL345** 3-Axis Accelerometer for motion detection and activity level analysis.
- **Key Breakthroughs:**
  - Designed and implemented a **Complementary/Kalman Filtering mechanism** using ADXL345 acceleration data to filter out motion artifacts and noise in optical PPG (MAX30102) readings.
  - Implemented low-latency **multithreaded task scheduling via FreeRTOS** to ensure real-time I2C sensor reading consistency without buffer overflows.
  - Built a lightweight BLE-GATT server to transmit physiological telemetry packs directly to a local web client.
- **Firmware Stack:** C++, FreeRTOS, ESP-IDF, I2C, Bluetooth Low Energy.

#### 🌉 ESP32 Structural Health Monitoring (SHM) System
An open-source, embedded IoT telemetry system designed to monitor bridges and civil structures for mechanical stress, extreme impacts, and dangerous road conditions.

- **The Objective:** Real-time structural safety telemetry (stable Pitch/Roll tilt, sudden G-force impacts, surface freezing warnings) streamed to cloud dashboards via MQTT.
- **Hardware Integration:**
  - **ESP32** dual-core processor managing low-latency data loops.
  - **MPU6050** 6-DOF IMU (Accelerometer & Gyroscope) for tilt and impact tracking.
  - **MLX90614** contactless infrared thermopile sensor for exact road surface temperature.
- **Key Breakthroughs:**
  - Designed and implemented a **Complementary Filter** to fuse gyroscope and accelerometer data to compute robust, drift-free Pitch and Roll angles.
  - Resolved **units mismatch errors** by converting MPU6050 gyroscope angular velocity from rad/s to deg/s ($\text{deg/s} = \text{rad/s} \times 180/\pi$) before integration.
  - Developed immediate edge-triggered notification flags (`IMPACT_DETECTED`, `TILT_LIMIT_EXCEEDED`, `SURFACE_ICE_WARNING`) sent via MQTT client.
- **Firmware Stack:** C++, Arduino Framework, PubSubClient (MQTT), I2C Protocol.

---

### 🛠️ Hardware & Systems Engineering

<details>
<summary><b>📐 Technical Core & Architecture</b></summary>
<br>

- **Languages:** C, C++ (Modern C++14/17 for embedded), Python.
- **Platforms/MCUs:** ESP32 (ESP-IDF / Arduino), STM32 (HAL / LL), STM32F4/F7, Arduino Core.
- **RTOS & Kernels:** FreeRTOS (Multi-tasking, Queues, Semaphores, Event Groups), bare-metal architectures.
- **Methodologies:** Low-power optimization, memory footprint reduction, interrupt-driven design, DMA (Direct Memory Access).
</details>

<details>
<summary><b>🔌 Connectivity & Protocols</b></summary>
<br>

- **Wired:** CAN Bus (Controller Area Network), I2C, SPI, UART/USART, OneWire.
- **Wireless:** BLE (Bluetooth Low Energy - Custom GATT, HID-over-GATT), Wi-Fi (ESP32 Station/AP, TCP/IP stack), MQTT, WebSockets.
- **Telemetry & Logging:** SD card logging, JSON serialization, edge-processing.
</details>

---

### 🚀 Interactive Projects

<details>
<summary><b>🏎️ RACEPULSE: ESP32 Endurance Race Car Telemetry</b></summary>
<br>
Real-time telemetry system designed for endurance motorsport applications.

- **Hardware:** ESP32-S3, CAN-bus transceiver, High-precision GPS module.
- **Features:** 
  - Live data streaming over MQTT/WebSockets.
  - On-board SD card logging for offline analysis.
  - Integrated lap-timing and tire temperature monitoring.
- **Stack:** C++, FreeRTOS, Grafana/InfluxDB for visualization.
</details>

<details>
<summary><b>🖱️ ESP32 Air Mouse: Wearable Gesture Controller</b></summary>
<br>
A wrist-mounted wearable that uses 6-axis IMU data to control cursors via BLE.

- **Hardware:** ESP32-C3, MPU6050 Accelerometer/Gyroscope.
- **Features:** 
  - HID-over-GATT (BLE) for driverless compatibility with Windows/macOS/Android.
  - Low-power optimization for extended battery life.
  - Complementary filter implementation for smooth cursor movement.
- **Stack:** C++, BLE-HID Library, Embedded Signal Processing.
</details>

---

### 📊 Performance Metrics & Activity

<p align="left">
  <img src="https://github-profile-trophy.vercel.app/?username=manideepreddyvangala04&theme=tokyonight&no-frame=true&margin-w=15" alt="GitHub Trophies" />
</p>

<p align="left">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=manideepreddyvangala04&theme=tokyonight" alt="GitHub Streak" />
</p>

---

### 🤝 Recruiter Quick-Connect

<details>
<summary><b>💼 Looking for an Embedded Systems Engineer? Expand here!</b></summary>
<br>

If you are a technical recruiter or hiring manager looking for a proactive firmware developer who loves hardware-software co-design, here is why we should connect:
- **Immediate Value:** I have hands-on experience building multi-sensor arrays, configuring real-time operating systems (FreeRTOS), and writing optimized C/C++ firmware.
- **My Toolset:** ESP-IDF, STM32CubeMX, PlatformIO, VS Code, Git/GitHub, Logic Analyzers, Oscilloscopes, and Multimeters.
- **Ready to Innovate:** Eager to tackle roles in IoT, wearable tech, automotive/motorsport systems, and biomedical instrumentation.

Let's discuss how my expertise in low-latency systems and RTOS can accelerate your team's hardware products!
</details>

<p align="center">
  <a href="https://linkedin.com/in/manideepreddyvangala04">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
</p>
