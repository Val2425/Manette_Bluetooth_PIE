# Schéma fonctionnel et connexions

## Vue d’ensemble
Le système se compose de trois sous-parties :
1. **Entrées** : joysticks et boutons
2. **Contrôleur** : ESP32-S3 (microcontrôleur principal)
3. **Alimentation et interface USB** : batterie, charge, port USB-C

## Alimentation
- Batterie Li-ion → Module TP4056 (charge)
- TP4056 OUT+ / OUT- → ESP32 5V et GND
- USB-C VBUS → TP4056 IN+
- USB-C GND → TP4056 IN-

## Contrôles
- Joysticks (KY-023)
  - VRx → GPIO 34 (entrée analogique)
  - VRy → GPIO 35 (entrée analogique)
  - SW → GPIO 18 (digital)

- Boutons → GPIO 19, 21, 22, 23, etc.

## Connexion USB/Bluetooth
- ESP32-S3 gère simultanément le mode HID Bluetooth et le port série USB.
- Sélection automatique selon l’état du câble USB.

> Un schéma Fritzing ou KiCad sera ajouté ici plus tard.
