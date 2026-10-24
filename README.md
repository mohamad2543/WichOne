# WichOne 🖥️
A lightweight, high-performance Windows floating HUD tool built in C++ to instantly monitor and display the active keyboard language (AR/EN) without cluttering your screen.

## ✨ Features
- **Floating HUD:** Always-on-top minimalist indicator in the top-right corner.
- **Position Toggle:** Easily switch the HUD position between the right and left sides of the screen.
- **Theme Switcher:** Toggle instantly between Dark and Light themes.
- **Global Hotkey:** Press `Ctrl + Shift + Q` to quickly hide or show the HUD.
- **System Tray Support:** Right-click the tray icon to access settings or exit safely.

## 🛠️ Compilation
Compile using `g++` with C++20 standard and Windows subsystem flags:
```bash
windres resource.rc -o resource.o
g++ -std=c++20 main.cpp resource.o -o WichOne.exe -luser32 -lgdi32 -lshell32 -static -mwindows