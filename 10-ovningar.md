
# Övningar

## Övning 1 - Spara tjänstelistan som JSON

Lägg till funktionerna `spara_tjanster` och `ladda_tjanster` i Service Status Tool. Testa att lägga till en tjänst, spara, stänga programmet och starta om - tjänsten ska fortfarande finnas kvar.

## Övning 2 - Läs in tjänstelistan vid start

Se till att `ladda_tjanster` anropas i programmets startsekvens och att det inte kraschar om filen inte finns.

## Övning 3 - Exportera statusrapport som CSV

Lägg till menyalternativet "Exportera rapport" och koppla det till funktionen `exportera_rapport`. Öppna den skapade CSV-filen i ett kalkylblad och kontrollera att den ser korrekt ut.

## Övning 4 - Läs konfiguration från fil

Skapa en `config.json` med inställningarna `datafil` och `rapportfil`. Läs in dem med `ladda_konfiguration` och använd dem i stället för hårdkodade filnamn. Testa att byta filnamn i `config.json` och kontrollera att programmet använder det nya namnet.

## Övning 5 - Hantera felformaterad JSON

Vad händer om `tjanster.json` innehåller felaktig JSON? Programmet kraschar med ett `json.JSONDecodeError`. Lägg till felhantering för det fallet och skriv ut ett tydligt felmeddelande i stället.

> Tips: `json.JSONDecodeError` är ett undantag som vi kan fånga med `except json.JSONDecodeError`.
