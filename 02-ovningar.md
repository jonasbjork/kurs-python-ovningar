# Övningar - Variabler, text och tal


## Övning 1 - Servernamn och status

Skriv ett program som lagrar ett servernamn och en status i variabler och sedan skriver ut:

```
Status för web-server-01: OK
```

Använd en f-string för utskriften.


## Övning 2 - Fyra datatyper

Skapa fyra variabler, en av varje typ: `str`, `int`, `float` och `bool`. Välj värden som passar i ett DevOps-sammanhang. Skriv sedan ut varje variabel tillsammans med dess datatyp med hjälp av `type()`.

## Övning 3 - Fråga användaren

Skriv ett program som frågar användaren efter ett servernamn och ett portnummer. Spara portnumret som ett heltal. Skriv sedan ut:

```
Ansluter till web-server-01 på port 8080...
```

Testa vad som händer om du skriver in text istället för ett tal i portnummerfältet.

## Övning 4 - Deployment-meddelande

Skriv ett program som frågar efter:

- applikationens namn
- version
- målmiljö (till exempel `dev`, `test` eller `prod`)
- vem som kör deploymenten

Programmet ska sedan skriva ut ett deployment-meddelande i stil med:

```
Deployment startar...
Applikation : my-app
Version     : 2.4.1
Miljö       : PRODUCTION
Utförs av   : anna
```

Miljönamnet ska skrivas ut med versaler. Snygga till formateringen så att kolumnerna är uppradade.

## Övning 5 - CPU-beräkning

Skriv ett program som frågar användaren om:

- antal CPU-kärnor på servern
- hur många kärnor en process använder (decimaltal)

Programmet ska räkna ut hur många processer som ryms och skriva ut svaret med ett tydligt meddelande, till exempel:

```
En server med 8 kärnor och 0.5 kärnor per process
klarar maximalt 16 processer.
```

