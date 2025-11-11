# Gestion de l’énergie

## Circuit de charge
- TP4056 avec protection intégrée
- Courant de charge : 1A max
- Diode de protection pour éviter le retour de courant vers USB

## Distribution
- Batterie → TP4056 → ESP32 5V → Régulateur interne 3.3V
- Port USB alimente aussi le système quand branché

## Objectif
- Pouvoir utiliser la manette en charge
- Prévoir indicateur LED pour niveau batterie et état de charge
