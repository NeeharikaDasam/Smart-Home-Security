# 📸 ESP32-CAM Image Capture and Save to SD Card

This project demonstrates how to use the **ESP32-CAM AI-Thinker module** to capture an image and save it directly to an SD card in JPEG format. The image is saved with a unique name (e.g., `picture1.jpg`, `picture2.jpg`, etc.) by using the EEPROM to store and increment the image number.

---

## ✅ Features

- Captures a photo using the ESP32-CAM on boot
- Saves the photo to a MicroSD card (1-bit SDMMC mode)
- Automatically names each image using EEPROM counter
- Uses onboard **LED Flash** while capturing the photo
- Enters **deep sleep** after saving the image
- Ready for battery-powered applications like wildlife cameras, remote sensing, etc.

---

## 🔧 Hardware Requirements

- [ESP32-CAM AI-Thinker](https://randomnerdtutorials.com/esp32-cam-ai-thinker-pinout/)
- MicroSD Card (tested with 2GB; supports up to 16GB)
- MicroSD Card Adapter (already included on ESP32-CAM)
- FTDI Programmer (for uploading code)
- Optional: External power source (for autonomous operation)

---

## 📷 Camera Configuration

This project is tailored for the **AI-Thinker model**:

```cpp
#define PWDN_GPIO_NUM     32
#define RESET_GPIO_NUM    -1
#define XCLK_GPIO_NUM      0
#define SIOD_GPIO_NUM     26
#define SIOC_GPIO_NUM     27
#define Y9_GPIO_NUM       35
#define Y8_GPIO_NUM       34
#define Y7_GPIO_NUM       39
#define Y6_GPIO_NUM       36
#define Y5_GPIO_NUM       21
#define Y4_GPIO_NUM       19
#define Y3_GPIO_NUM       18
#define Y2_GPIO_NUM        5
#define VSYNC_GPIO_NUM    25
#define HREF_GPIO_NUM     23
#define PCLK_GPIO_NUM     22
