# Manette Bluetooth + USB

**Projet DIY de manette personnalisée** avec :
- PCB custom
- ESP32-S3
- Connexion Bluetooth & USB
- Batterie rechargeable (une seule prise USB pour charge et données)
- Boîtier imprimé en 3D

---

## Objectif

Ce projet a pour but de concevoir une **manette fonctionnelle et documentée de A à Z**, en suivant une démarche d’ingénierie complète :
- Étude électronique
- Schéma et PCB
- Programmation du firmware (Bluetooth HID + USB HID)
- Gestion d’énergie et charge
- Design mécanique et impression 3D
- Tests et validation

Le projet est pensé pour être **pédagogique et reproductible**.

---

## Composants principaux

| Fonction | Composant | Lien |
|-----------|------------|------|
| Microcontrôleur | ESP32-S3 DevKitC | [Amazon](https://www.amazon.fr/dp/B0DG8L1YW9) |
| Joystick | KY-023 | [Amazon](https://www.amazon.fr/dp/B07WTYSGSC) |
| Circuit de charge | TP4056 / MCP73871 | [AliExpress](https://fr.aliexpress.com/item/1005002877455453.html) |
| Batterie | Li-ion 3.7V | — |
| Port USB-C | Module USB-C breakout | — |
| Boutons | Tact switch 12x12 mm | [AliExpress](https://fr.aliexpress.com/item/1005005237733531.html) |

*(Voir `docs/02_Components.md` pour la liste complète et les schémas.)*

---

## Fonctions prévues

- 2 joysticks + 10 boutons
- Batterie rechargeable via USB
- Mode USB : HID (manette filaire)
- Mode Bluetooth : HID sans fil
- Bascule automatique entre USB et Bluetooth
- Boîtier imprimé en 3D

---

## Documentation

La documentation complète du projet est disponible dans [`/docs`](docs/).

- [01 - Objectif](docs/01_Objectif.md)
- [02 - Composants](docs/02_Components.md)
- [03 - Schéma électronique](docs/03_Schema.md)
- [04 - Prototypage](docs/04_Prototypage.md)
- [05 - Code & Firmware](docs/05_Code.md)
- [06 - Gestion d’énergie](docs/06_Energie.md)
- [07 - Boîtier 3D](docs/07_Boitier3D.md)
- [08 - Tests & Validation](docs/08_Tests.md)

---

## Environnement de développement

- **IDE :** Arduino IDE / PlatformIO  
- **Langage :** C++ (Arduino Framework)  
- **Carte :** ESP32-S3 DevKitC  
- **Librairies :**
  - `ESP32 BLE HID`
  - `USBHost`
  - `AnalogJoystick`

---

## Auteur

Projet initié et documenté par **Valentin Girold**, dans une démarche d’apprentissage en électronique, design et ingénierie logicielle.

---

## Licence

Ce projet est sous licence **MIT** — libre à l’usage, modification et distribution.
