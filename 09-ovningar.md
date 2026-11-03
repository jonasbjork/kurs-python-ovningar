
# Övningar

## Övning 1 - Läs en loggfil

Skapa en textfil som heter `tjanst.log` med följande innehåll:

```
2025-03-01 09:00:00 INFO  service started
2025-03-01 09:01:12 INFO  health check OK
2025-03-01 09:02:45 ERROR failed to connect to database
2025-03-01 09:03:00 INFO  retrying connection
2025-03-01 09:03:05 ERROR database connection timeout
2025-03-01 09:04:00 INFO  connection restored
```

Skriv ett Python-skript som läser filen och skriver ut alla rader till terminalen.

## Övning 2 - Räkna rader

Utöka skriptet från övning 1 så att det också skriver ut hur många rader filen
innehåller.

Förväntad utskrift:

```
Loggfilen innehåller 6 rader.
```

## Övning 3 - Hitta rader med fel

Utöka skriptet ytterligare så att det hittar och skriver ut alla rader som
innehåller `ERROR`.

Förväntad utskrift:

```
Hittade 2 felrader:
  2025-03-01 09:02:45 ERROR failed to connect to database
  2025-03-01 09:03:05 ERROR database connection timeout
```

## Övning 4 - Skriv en rapport till fil

Skapa ett skript som:

1. Läser `tjanst.log`
2. Räknar totalt antal rader
3. Hittar alla felrader
4. Sparar en sammanfattning till en fil som heter `logg-rapport.txt`

Filen ska se ut ungefär så här:

```
=== Loggrapport ===
Totalt antal rader: 6
Antal felrader: 2

Felrader:
2025-03-01 09:02:45 ERROR failed to connect to database
2025-03-01 09:03:05 ERROR database connection timeout
```
## Övning 5 - Service Status Tool

Utöka *Service Status Tool* från föregående kapitel med en funktion
`spara_rapport(filnamn)` som sparar en lista med tjänster och deras status
till en textfil.

Tänk på att:

- använda `with open(...)`
- skriva ut ett bekräftelsemeddelande när rapporten har sparats

## Extraövning

Skriv ett skript som:

1. Frågar användaren efter ett filnamn med `input()`
2. Läser filen
3. Räknar hur många rader som innehåller `INFO`, `WARNING` respektive `ERROR`
4. Skriver ut en sammanfattning

Förväntad utskrift för `tjanst.log`:

```
=== Loggsummering för tjanst.log ===
INFO:    4 rader
WARNING: 0 rader
ERROR:   2 rader
```

Kontrollera om filen finns innan den läses in och skriv ut ett tydligt
felmeddelande om den saknas.

> **Tips:** Längre fram lär vi oss ta emot filnamnet som ett
> kommandoradsargument i stället för med `input()` och hantera saknade filer
> med `try`/`except` och exit-koder. Just nu räcker det med `input()` och ett
> enkelt villkor.
