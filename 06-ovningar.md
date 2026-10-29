# Övningar - Miniprojekt

## Övning 1 - Kör programmet

Skapa filen `service_status.py`, klistra in koden och kör den. Testa alla fem menyalternativen. Lägg till minst en tjänst och ändra status på en befintlig.

## Övning 2 - Lägg till en egen tjänst

Lägg till ytterligare en tjänst i startvärdet för `tjanster` i `main()`. Välj ett namn och en status själv.

## Övning 3 - Enkel rapport

Lägg till ett sjätte menyalternativ: `6. Visa rapport`. Rapporten ska räkna hur många tjänster som har status `running`, hur många som har `stopped` och hur många som har `unknown` och skriva ut sammanfattningen:

```
--- Rapport ---
  Running:  2
  Stopped:  1
  Unknown:  0
```

> **Tips:** Använd en loop och räkna med variabler. Skapa en ny funktion `visa_rapport(tjanster)` och anropa den från `main()`.

## Övning 4 - Validera status

Just nu kan användaren skriva vilken status som helst när hon ändrar en tjänst. Lägg till en kontroll i `andra_status()` som bara accepterar `running`, `stopped` eller `unknown`. Om användaren skriver något annat ska programmet skriva ut ett felmeddelande och be om ny inmatning.

> **Tips:** En `while True`-loop inuti funktionen kan vara praktisk här.

