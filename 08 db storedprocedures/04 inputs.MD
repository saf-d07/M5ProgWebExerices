## STP input

- lees het volgende:
```
Een stored procedure is krachtig omdat het net als `functions` `argumenten kan hebben

Dat maakt Select ... Where mogelijk
OF insert ... into 
```

## nieuwe STP

- lees de opdracht:
```
we gaan een nieuwe STP maken: Een zoek in je bookmarks STP
```

- maak de STP, noem deze:
    - searchBookmark
- maak de select statement op de webbookmarks
    - zorg dat je een `where` hebt die zoekt in `sitename` EN `link`
- gebruik nu even vaste waardes achter de =
    - bv 'dummy'
- bewaar SQL in een aparte SQL file met goede naam

## EXTRA:
- probeer een `LIKE` proberen
    - dan heb je ook `concat` nodig om de "%" met je argument in een string te zetten

## rechten

- geef meteen even je user `appStpUser` rechten op de STP
- en sla dat op bij de SQL file 


## argumenten

- bekijk de code hieronder:
```SQL 
CREATE PROCEDURE `emailById` ( in id Int, in afterGuid varchar(36))
```

- lees de uitleg:
```
* deze heeft `2` argumenten (id en afterGuid)
* die staan `tussen` haakjes `achter` de `naam`
* elk argument heeft `in` ervoor
* elk argument heeft het `type` erachten (int & varchar(36))
```
- geef nu jouw STP `1 argument` van het type `varchar`, bedenk zelf hoeveel characters handig is

## argument gebruiken

> !! deze statement is even in elkaar gefrommeled.
- lees de code hieronder, waar worden de argumenten gebruikt?

```SQL

select * from email where idemail = id and idemail > (select id from email where guid = afterGuid)
```

- gebruik nu jouw argument in jouw STP `searchBookmark` zodat deze zoekt
- bewaar SQL in een aparte SQL file met goede naam


## git

commit de .sql file + de screenshots naar je git repository voor de vak!