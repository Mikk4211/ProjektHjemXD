## ProjektHjemXD

# _Mathias:_ 

1. Ass-Pounder 8000 - turn on the ass-pounder 8000 ;]

2. Kaffe maskine - Wifi-kontrolleret kaffemaskine, der tænder for din kaffemaskine når du trykker i en app

3. Temperatursensor - Tjekker temperaturen i rummet, og vil tjekke om temperaturen er tilpas, skal skrues op eller ned. 

4. Klappesensor - Tænder eller slukker for lyset, når der bliver klappet i huset. 

5. Støvsugerrobotter - WIP

## _Klasser:_

# 1. _Støvsugerrobotter:_

StøvsugerTænd, StøvsugerSluk 

Sensor.java

Boolean (Er mennesket tilstede)

# 2. _Temperaturcensor:_

TemperaturOp, TemperaturNed, TemperaturMåler

Sensor.java

Boolean (Er vinduet åbent - censor til dette også)

# 3. _Klappecensor:_

Sensor.java

LysTænd, LysSluk

En form for lyddetektor til at se om der bliver klappet, evt en counter til hvor mange klap der bliver klappet. 

# 4. _Kaffemaskine m/ wifi:_

          ~KaffemaskineApp.java~

KaffemaskineTænd, KaffemaskineSluk, KaffemaskineVolumen

En form for wifi-modul, som skal gøre det modulet at starte kaffemaskinen vha. en app på din telefon. 

# 5. _Ass-pounder 8000:_

evt app til at bestille mad til dig in the act?? xdddxdd
TBD, WIP

## Abstractions / Re-usability: 

Sensor.java kan i hvert fald genbruges gennem flere forskellige klasser, da det ikke er låst fast til sensoren at have en funktion. 
Vi kan f.eks. have én sensor til at måle både temperatur, og se om lyset er tændt, i stedet for at have flere forskellige sensore. Støvsugerrobboterne skal nok have en seperat 'sensor', da denne funktion sandsynligvis skulle være bundet til en form for GPS, som arbejder sammen med din telefon. 

Resten af funktionerne skal bruges hver for sig, da disse låses fast til et enkelt objekt (StøvsugerTænd, LysTænd) - men disse ville kunne laves i en seperat klasse med én metode, som tænder. 

