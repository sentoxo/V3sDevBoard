# V3sDevBoard
Educational project of first PCB desgin, SBC with linux built on allwinner V3s SoC.  
Work in progress.  
Phase 1 - Research and drawing schematics in kicad, 22-30dec  
Phase 2 - PCB design, 28.01-05.02

![image](https://github.com/sentoxo/V3sDevBoard/blob/main/photo.png)

## SYSTEM SPECIFICATIONS
=====================

### CORE SYSTEM:
- CPU: Allwinner V3s (ARM Cortex-A7 @ 1.2GHz)
- RAM: 64MB DDR2 @ 400MHz (Integrated SiP)
- STORAGE: SD Interface for OS (SDIO compatible)

### CONNECTIVITY:
- ETHERNET: 100Mbps Interface
- WIRELESS: WiFi & Bluetooth (via ESP32[ESP-Hosted-NG] on SDIO/UART) {PG0-5 -> SDIO, PB0-1 -> UART}
- LONG RANGE: LoRa support (via Ra-02 on SPI) {PB2 -> RESET, PB3 -> INT, PC0-3 -> SPI}
- USB: USB Host support (Simple)
- DEBUG: System UARTs to USB bridge

### DISPLAY & IMAGING:
- CAMERA: MIPI CSI (22-pin connector)
- LCD: RGB-666 Interface with backlight support (40-pin) [ST7280] {PB4 -> LC_LED_PWM, PE0-19,23-24}

### SENSORS & I/O:
- MOTION: MPU6050 Accelerometer & Gyroscope [I2C] {PB6-7}
- ENVIRONMENT: BME280 Sensor (Temp/Press/Hum) [I2C] {PB6-7}
- AUDIO: 3.5mm Audio Jack
- INPUT: Low-resolution ADC for button matrix (6 buttons)
- VISUAL: PCB RGB backlight WS2812B {PB5}

### POWER & SOFTWARE:
- REGULATION: DC-DC converters for 3.3V, 1.8V, 1.2V
- OPERATING SYSTEM: Powered by custom Mainline Linux
