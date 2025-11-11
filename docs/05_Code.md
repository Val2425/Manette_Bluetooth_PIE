# Organisation du code

## Structure
Le code sera organisé comme suit :
src/
├── main.ino
├── joystick.cpp / joystick.h
├── buttons.cpp / buttons.h
├── usb_manager.cpp / usb_manager.h
└── bluetooth_manager.cpp / bluetooth_manager.h

## Fonctionnalités principales
- Lecture des entrées
- Transmission HID Bluetooth ou USB
- Gestion de la batterie (niveau et charge)
- Mode veille si inactif

## Librairies utiles
- `BluetoothSerial.h`
- `ESP32 HID library`
- `Wire.h` / `Adafruit_Sensor.h` si capteurs ajoutés

