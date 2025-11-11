# Prototypage

## Étape 1 : Joystick
- Test de lecture analogique sur les axes X et Y
- Test du bouton “clic” intégré
- Vérification des tensions de sortie (0–3.3V)

## Étape 2 : Boutons
- Test de la détection avec `digitalRead()`
- Ajout de résistances pull-down si nécessaire

## Étape 3 : Alimentation
- Vérifier la tension de sortie du TP4056 (5V → 3.7V → ESP32)
- Contrôle de la recharge de la batterie

## Étape 4 : Communication USB/Bluetooth
- Test HID Bluetooth (reconnaissance comme manette sur PC)
- Test port série USB pour communication en mode filaire
