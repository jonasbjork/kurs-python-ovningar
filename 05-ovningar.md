# Övningar - Listor

## Övning 1 - En lista med servrar

Skapa en lista med minst fem servernamn. Skriv sedan ut varje servernamn med en `for`-loop:

```
Servern web-01 är registrerad.
Servern web-02 är registrerad.
...
```

Skriv också ut hur många servrar det finns totalt, till exempel:

```
Totalt: 5 servrar
```

## Övning 2 - En dictionary med tjänstinformation

Skapa en dictionary för tjänsten `sshd` med följande information:

- namn: `sshd`
- status: `running`
- port: `22`
- protokoll: `tcp`

Skriv sedan ut all information med en `for`-loop och `.items()`, på formatet:

```
namn: sshd
status: running
port: 22
protokoll: tcp
```

## Övning 3 - Statusrapport

Skapa en lista med minst fyra tjänster som dictionaries. Varje dictionary skall ha minst `namn` och `status`. Skriv en `for`-loop som:

- skriver ut `[OK]` om status är `running`
- skriver ut `[FEL]` om status är något annat

## Övning 4 - Lägg till och ta bort

Börja med en lista med tre tjänstenamn. Gör sedan följande steg och skriv ut listan efter varje steg:

1. Lägg till en fjärde tjänst med `append()`.
2. Ta bort den andra tjänsten med `remove()`.
3. Skriv ut hur många tjänster som finns kvar med `len()`.

## Övning 5 - Kombinera lista och dictionary

Skapa en lista med minst fem tjänster som dictionaries. Lägg till ett extra fält, `"svar_tid_ms"`, med ett heltal som representerar svarstid i millisekunder.

Skriv ett program som:

1. Skriver ut alla tjänster med status och svarstid.
2. Räknar hur många tjänster som har status `"running"`.
3. Skriver ut namnet på den tjänst som har högst svarstid.

> Tips: Titta på hur vi kan använda en vanlig variabel för att hålla koll på maxvärdet när vi loopar igenom listan.
