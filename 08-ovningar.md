
# Övningar - Moduler

## Övning 1 - Dela upp ett litet program

- Skapa en ny katalog `litet-program`
- Skapa tre filer: `main.py`, `halsning.py` och `info.py`.

I `halsning.py` skriver du en funktion `visa_halsning()` som skriver ut:

```
Hej fran Service Status Tool!
```

I `info.py` skriver du en funktion `visa_version()` som skriver ut:

```
Version: 1.0
```

I `main.py` importerar du båda modulerna och anropar funktionerna.


## Övning 2 - Dela upp Service Status Tool

Ta det Service Status Tool-skript vi har byggt i tidigare kapitel och dela upp det i
minst två filer:

- `tjanster.py` - data och logik
- `main.py` - startar programmet

Se till att `main.py` importerar och använder funktioner från `tjanster.py`.

Lägg till `if __name__ == "__main__":` i `main.py`.


## Övning 3 - Lägg till en utskriftsmodul

Utöka projektet med en tredje fil: `utskrift.py`.

Flytta alla `print()`-anrop från `tjanster.py` till funktioner i `utskrift.py`.

Importera och använd `utskrift` i `main.py`.


## Övning 4 - Skriv en README.md

Skriv en enkel `README.md` för Service Status Tool.

Den ska innehålla:

- En rubrik med projektets namn
- En kort beskrivning av vad det gör
- Instruktioner för hur man kör det
- En lista över filerna i projektet och vad de gör


## Övning 5 - Utforska ett riktigt projekt

Gå till GitHub.com (med din webbläsare) och sök efter ett litet Python-projekt - gärna ett DevOps-relaterat verktyg. Titta på hur det är strukturerat:

- Hur många filer finns det?
- Finns det en `README.md`?
- Finns det en `requirements.txt`?
- Hur är koden uppdelad?

Det behöver inte vara ett komplicerat projekt. Syftet är att börja se hur andra
organiserar sin kod.

