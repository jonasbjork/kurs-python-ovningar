# Övningar

## Övning 1 - Skriv ut aktuell tid i en rapport

Skriv ett skript som skriver ut en enkel statusrapport med aktuell tidsstämpel:

```
=== Statusrapport ===
Genererad: 2025-03-14 09:45:23

Tjänster som kontrolleras:
- nginx
- postgresql
- redis
```

Tips: Använd `datetime.now().strftime()` för att formatera tidsstämpeln.

## Övning 2 - Utforska arbetsmiljön

Skriv ett skript som skriver ut vilket operativsystem programmet körs på (`os.name`) och vilken katalog det körs ifrån (`os.getcwd()`). Skapa sedan en ny katalog som heter `rapporter` med `os.mkdir()`.

> Kör skriptet två gånger. Vad händer andra gången, när katalogen redan finns? Det är precis den typen av fel `pathlib` hanterar lite smidigare, som vi nämnde tidigare i kapitlet.

## Övning 3 - Kontrollera om en fil finns

Skriv ett skript som frågar användaren efter ett filnamn med `input()` och kontrollerar om filen finns, till exempel med `pathlib.Path(filnamn).exists()`. Skriptet ska:

- Skriva ut ett positivt meddelande om filen finns
- Skriva ut ett felmeddelande och avsluta med exitkod `1` med `sys.exit(1)` om filen saknas

Testa med en fil som finns och en som inte finns.

> Längre fram lär vi oss ta emot filnamnet som ett kommandoradsargument i stället för med `input()`.

## Övning 4 - Kör ett enkelt systemkommando

Skriv ett skript som kör kommandot `uptime` med `subprocess.run()` och skriver ut resultatet. Skriptet ska också skriva ut exitkoden.

Utöka sedan skriptet så att det också kör `df -h` och skriver ut diskanvändningen.

## Övning 5 - Prova `logging` för första gången

Ta ett skript vi skrivit tidigare i kursen, till exempel statusrapporten från övning 1 här ovanför, och byt ut `print()`-anropen mot `logging.info()`. Lägg till `logging.basicConfig(level=logging.INFO)` överst i skriptet så att meddelandena visas.

Det här är bara en första bekantskap med `logging`. Vi kommer gå igenom modulen ordentligt senare och lär oss skriva loggar både till terminalen och till fil, med olika nivåer för olika typer av meddelanden.
