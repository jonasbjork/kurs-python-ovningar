
# Övningar - Loopar

## Övning 1 - Skriv ut status för flera servrar

Skapa en lista med minst fem servernamn. Loopa igenom listan och skriv ut ett meddelande för varje server. Använd `f`-strängar för att göra utskriften läsbar.

Exempel på utdata:

```
Kontrollerar server: web01
Kontrollerar server: web02
Kontrollerar server: db01
...
```

**Utmaning:** Lägg till en räknare som håller koll på hur många servrar som kontrollerats. Skriv ut totalen när loopen är klar.

## Övning 2 - Bygg en meny

Skapa ett menyprogram med minst tre val. Menyn ska visas om och om igen tills användaren väljer att avsluta. Ogiltiga val ska ge ett vänligt felmeddelande.

Välj gärna val som känns relevanta - till exempel "Visa serverstatus", "Rensa skärmen" och "Avsluta".

## Övning 3 - Simulera en hälsokontroll

Skapa en lista med dictionaries, där varje dictionary representerar en tjänst med ett namn och en status. Loopa igenom listan och skriv ut:

- `OK` om tjänsten har status `"igång"`
- `VARNING` om den har någon annan status

Räkna hur många tjänster som är igång och hur många som inte är det. Skriv ut en sammanfattning i slutet:

```
Sammanfattning: 3 av 4 tjänster är igång.
```

**Utmaning:** Använd `continue` för att hoppa över tjänster som har status `"underhall"` och inte räkna in dem i vare sig OK eller VARNING.
