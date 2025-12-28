# V3sDevBoard
Educational project of first PCB desgin, SBC with linux built on allwinner V3s SoC.
Work in progress.
Phase 1 - Research and drawing schematics in kicad, 22-28dec
Phase 2 - PCB design, 28-


## SYSTEM SPECIFICATIONS
=====================

### CORE SYSTEM:
- CPU: Allwinner V3s (ARM Cortex-A7 @ 1.2GHz)
- RAM: 64MB DDR2 @ 400MHz (Integrated SiP)
- STORAGE: SD Interface for OS (SDIO compatible)

### CONNECTIVITY:
- ETHERNET: 100Mbps Interface
- WIRELESS: WiFi & Bluetooth (via ESP32)
- LONG RANGE: LoRa support (via Ra-02)
- USB: USB Host/OTG support
- DEBUG: System UARTs to USB bridge

### DISPLAY & IMAGING:
- CAMERA: MIPI CSI (22-pin connector)
- LCD: RGB-666 Interface with backlight support (40-pin)

### SENSORS & I/O:
- MOTION: MPU6050 Accelerometer & Gyroscope
- ENVIRONMENT: BME280 Sensor (Temp/Press/Hum)
- AUDIO: 3.5mm Audio Jack
- INPUT: Low-resolution ADC for button matrix
- VISUAL: PCB RGB backlight

### POWER & SOFTWARE:
- REGULATION: DC-DC converters for 3.3V, 1.8V, 1.2V
- OPERATING SYSTEM: Powered by custom Mainline Linux