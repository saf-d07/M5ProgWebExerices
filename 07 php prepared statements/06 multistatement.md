## Gevaar ervaren

Die multistatements, kennen we die nog?

laten we daar het gevaar ook testen


## start

- maak een `gehacked.php` naar `multistatement.php`
- in die file werken we

## stap 1

- lees het volgende:
```
we gaan de mysql query uitvoering nu aanpassen naar `multi_statements`
* https://www.php.net/manual/en/mysqli.quickstart.multiple-statement.php
```
- pas het aan
- test of je code het nog doet en resultaat geeft

## hacken

- lees het volgende:
```
nu gaan we 'hacken', als we de volgende url gebruiken:
* http://localhost:88/multistatement.php?search=mario or naam like 'sonic`

krijgen we 2 resultaten
maar we kunnen nog meer omdat we nu een `multi_statements` hebben:
* we mogen nu `;` gebruiken om meerdere sql queries te doen 
```

- http://localhost:88/multistatement.php?search=mario';SELECT table_name FROM information_schema.tables;

- wat krijg je nu voor resultaten? `Screenshot` dat even!


## Notes

- lees het volgende:
```
* een prepared statement kan geen multi query zijn
* als je een multi statement nodig hebt => neem `geen` user input aan. 
* Er zijn andere oplossingen, maar dat komt later met Stored procedures
* behandel elke query in je code met user input als onveilig.
```

## git

commit je files naar je git repository voor de vak!