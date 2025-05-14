## 🔧 Features

* Displays a monochrome image (converted to byte array) on an OLED display.
* Utilizes the I2C protocol for communication between ESP32 and OLED (SDA, SCL).
* Ideal for digital ID cards, mini dashboards, or simple photo frames.

## 🧰 Hardware Used

* ESP32 Dev Board
* 0.96" I2C OLED Display (SSD1306)

## 💡 How It Works

1. A photo is converted into a monochrome bitmap using tool like "Image2CPP**"
2. The image data is stored in a byte array ('const unsigned char image[] PROGMEM = { ... };').
3. The image is drawn on the screen using the 'Adafruit_SSD1306' library.

## 🧪 Libraries Used

* [Adafruit SSD1306](https://github.com/adafruit/Adafruit_SSD1306)
* [Adafruit GFX](https://github.com/adafruit/Adafruit-GFX-Library)

## 🚀 Getting Started

 Connect the OLED to the ESP32:

   * VCC → 3.3V
   * GND → GND
   * SCL → GPIO 22
   * SDA → GPIO 21

## 🧠 Learnings

* Image-to-byte conversion for embedded displays.
* I2C OLED communication with ESP32.
* Display buffer management in constrained environments.

## 🙌 Acknowledgments

Thanks to open-source tools and the Adafruit libraries that made this simple image rendering possible on microcontrollers.
