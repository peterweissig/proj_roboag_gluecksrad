# Glücksrad


**Allgemein**
-------------
- Preise
    - es gibt insgesamt 5 verschiedene Preiskategorien:
        - 1: 300x, blau
        - 2: 150x, grün
        - 3: 150x, rot
        - 4:  15x, gelb
        - 5:   5x, weiß
    - die Wahrscheinlichkeiten sind im besten Fall im Verhältnis von Anzahl zu Preissumme verteilt
- Buttons:
    - es gibt insgesamt zwei Buttons:
        - Bumper: extern am Glücksrad anzuschließender Riesenknopf
        - Mode:   kleiner, roter, an der Rückseite des Glücksrades befestigter Knopf



**Modi:**
---------
- Standard
    - die Preisverteilung entspricht den Standard-Werten und bleibt konstant
- Lenz
    - die Wahrscheinlichkeiten werden nach jedem Dreh neu entsprechend der Anzahl verbleibenden Preise verteilt
    - wenn alle Preise verteilt wurden (Summe der verbleibenden Preise = 0) wird dies durch eine Blink-Animation in den normalen Preisfarben kundgetan



**Drehen:**
-----------
- durch Drücken auf den Bumper im Demo-Modus wird die Dreh-Animation zu einem zufälligen Feld ausgelöst
- danach leuchten die LEDs in 3 verschiedenen Animationen (je nach Preisklasse) in der erdrehten Farbe auf
- während beider Vorgänge ist der Bumper blockiert
- durch drücken des Mode-Buttons wird die Animation beendet und der Bumper freigegeben



# Menü-Implementierung


**Start:**
----------
- es wird der letzte Glücksrad-Modus geladen, ggf. die gespeicherte Preisliste
- der geladene Modus wird durch 1-sekündiges Leuchten aller LEDs angezeigt:
    - grün: Standard
    - gelb: Lenz
- es startet die Demo-Animation



**Menü:**
---------
- durch 3-sekündiges Drücken des Mode-Buttons im Demo-Modus oder während der 'Preise-Leer' Animation wird das Menü angezeigt
- Navigiert wird mithilfe des Mode-Buttons
- Ausgewählt wird durch 3-sekündiges Drücken auf den Bumper
- zurzeit gibt es 4 Menüpunkte:
    - Blau: beendet das Menü ohne eine Aktion
    - Grün: wechselt in den Standard-Modus
    - Gelb: wechselt in den Lenz-Modus
    - Rot : resettet die Preisliste
