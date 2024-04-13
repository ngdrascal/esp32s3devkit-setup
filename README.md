# esp32s3devkit-setup
<h3>Settings and configurations needed to use the debugger in VS Code/PlatformIO with ESP32-S3-DevKitC-1.</h3>

---
#### ESP32-S3-DEVKITC-1
<image src=./images/esp32-s3-devkitc-1.png height=50% width=60% alt="ESP32-S3-DEVKITC-1">

---
#### Zadig - Silicon Labs CP210x USB to UART Bridge
<image src="./images/usb_to_uart.png" height=50% width=50% alt="Silicon Labs CP210x USB to UART Bridge">

---
#### Zadig - USB JTAG/serial debug unit (Interface 0)
<image src="./images/jtag_interface0.png" height=50% width=50% alt="USB JTAG/serial debug unit (Interface 0)">

---
#### Zadig - USB JTAG/serial debug unit (Interface 2)
<image src="./images/jtag_interface2.png" height=50% width=50% alt="USB JTAG/serial debug unit (Interface 2)">

---
#### Device Manager - Ports (COM & LPT)
<image src="./images/device_manager_usb_to_uart.png" height=50% width=50% alt="Silicon Labs CP210x USB to UART Bridge">

---
#### Device Manager - Universal Serial Bus devices
<image src="./images/device_manager_jtag.png" height=50% width=50% alt="Silicon Labs CP210x USB to UART Bridge">

---
```ini
; PlatformIO Project Configuration File
;
;   Build options: build flags, source filter
;   Upload options: custom upload port, speed and extra flags
;   Library options: dependencies, extra library storages
;   Advanced options: extra scripting
;
; Please visit documentation for the other options and examples
; https://docs.platformio.org/page/projectconf.html

[env:esp32-s3-devkitc-1]
platform = espressif32
board = esp32-s3-devkitc-1
framework = espidf
build_type = debug
upload_protocol = esp-builtin
monitor_port = COM8
monitor_speed = 115200
debug_tool = esp-builtin
