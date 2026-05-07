# Bingo

Eine statische Bingo-Board-Website, die alle Eingaben über Firebase Realtime Database synchronisiert.

## Firebase

Die Website nutzt die Firebase-Konfiguration aus `index.html` und speichert das gemeinsame Board unter dem Realtime-Database-Pfad:

```text
bingo/sharedBoard
```

Damit alle Besucher dasselbe Board lesen und schreiben können, müssen die Firebase Realtime Database Rules für diesen Pfad Lese- und Schreibzugriff erlauben. Ohne passende Rules zeigt die Website einen Firebase-Fehlerstatus an und behält nur die lokale Browser-Kopie.
