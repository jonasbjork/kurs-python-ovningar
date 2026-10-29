
# Övningar - Villkor

## Övning 1 - Statuskontroll

Skapa ett skript som heter `statuskontroll.py`. Skriptet ska:

1. Spara en status i en variabel - välj själv om det ska vara `"OK"`,
   `"WARNING"` eller `"ERROR"`
2. Använda `if`, `elif` och `else` för att skriva ut ett lämpligt meddelande
   för varje status
3. Ha ett `else` som hanterar okända statusvärden

Testa skriptet med alla fyra möjliga värden (inklusive ett påhittat sådant
som `"UNKNOWN"`).

## Övning 2 - Deploy-skydd

Skapa ett skript som heter `deploy_check.py`. Skriptet ska:

1. Ha en variabel `miljo` som kan vara `"dev"`, `"staging"` eller `"prod"`
2. Om miljön är `"prod"` ska skriptet skriva ut en tydlig varning och fråga
   om bekräftelse med `input()`
3. Om miljön är `"dev"` eller `"staging"` ska deploy starta direkt (en enkel
   utskrift räcker)
4. Om miljön är något annat ska skriptet skriva ut ett felmeddelande

## Övning 3 - HTTP-statuskod

Skapa ett skript som heter `http_check.py`. Skriptet ska:

1. Spara en HTTP-statuskod i en variabel, till exempel `200`, `301`, `404`
   eller `500`
2. Använda `if`, `elif` och `else` med numeriska jämförelser för att
   kategorisera koden:
   - 200-299: lyckad
   - 300-399: omdirigering
   - 400-499: klientfel
   - 500 och uppåt: serverfel

## Övning 4 - Bygg ett enkelt menyval

Skapa ett skript som heter `meny.py`. Skriptet ska:

1. Visa tre alternativ:
   ```
   1. Visa tjänststatus
   2. Visa miljö
   3. Avsluta
   ```
2. Ta emot ett val med `input()`
3. Använda `if`, `elif` och `else` för att reagera på valet

Det spelar ingen roll vad skriptet skriver ut för varje val i den här övningen -
det viktiga är att valen leder till olika utskrifter.

> **Tips:** Värdet från `input()` är alltid en sträng. Jämför därför med
> `"1"`, `"2"` och `"3"` - inte med siffrorna `1`, `2` och `3`.

