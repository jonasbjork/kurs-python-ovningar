
# Övningar - Funktioner

## Övning 1 - Flytta kod till funktioner

Ta koden från ditt mini-projekt i kapitel 6 och organisera om den med funktioner. Skapa minst tre funktioner (från den befintliga koden) och se till att varje funktion gör en tydlig sak.

## Övning 2 - check_service()

Skapa en funktion som heter `check_service()`. Den ska ta emot två parametrar: `name` och `status`. Om status är `"OK"` skrivs `[OK]` ut. Om status är `"FEL"` skrivs `[FEL]` ut. Testa med minst tre olika tjänster.

Exempel på utdata:

```
[OK]  nginx
[FEL] postgres
[OK]  redis
```

### Övning 3 - print_report()

Skapa en funktion som heter `print_report()`. Den ska ta emot en lista med tjänster och anropa `check_service()` för varje tjänst. Lägg till en rubrik och en avgränsningslinje.

Testa med den här listan:

```python
services = [
    {"name": "nginx", "status": "OK"},
    {"name": "postgres", "status": "FEL"},
    {"name": "redis", "status": "OK"},
]
```

### Övning 4 - validate_choice()

I kapitel 5 byggde vi en meny med `input()`. Nu ska vi skapa en funktion som heter `validate_choice()`. Den tar emot det användaren har skrivit och en lista med giltiga val. Den returnerar `True` om valet är giltigt och `False` om det inte är det.

```python
def validate_choice(choice, valid_choices):
    # Din kod här
    pass

print(validate_choice("1", ["1", "2", "3"]))  # True
print(validate_choice("9", ["1", "2", "3"]))  # False
```

### Övning 5 - Sätt ihop allt

Skapa ett skript med minst fyra funktioner: `get_services()`, `check_service()`, `print_report()` och `main()`. Skriptet ska köra `main()` när det startar. Försök också lägga till en enkel meny där användaren kan välja att visa rapporten eller avsluta.



