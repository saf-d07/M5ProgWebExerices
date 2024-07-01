## Users

we gaan nu kijken of de rechten kloppen

## workbench

- start mysql workbench
- log in met je M5ProgDocker connection

## table maken

- maak in `m5prog` een table `test`
- geef deze 1 colomn
>![](img/table.PNG)

## inloggen met de gebruiker

- ga naar de home tab (het huisje)
- click de `+` en vul je `m5progweb` gebruiker in
- test de connectie
- open nu de connectie

## select

als het goed is mogen we selecteren
- select alles van de table `test`

krijg je geen fouten? mooi! dan werkt het
- maak een screenshot van het resultaat
    - sla deze op onder je M5ProgWebC24 map
        - met de naam `02 appusertest.png`


## Admin

- maak een nieuwe connection maar dan met `M5ProgDocker`
> elke tab die opend heeft zijn eigen connection en dus eigen rechten!
- open de gebruiker `m5progweb`
- verander de rechten naar alleen `insert`

## select

als het goed is mogen we nu niet meer selecteren
- select alles van de table `test`

krijg je een fouten? mooi! dan werkt het
- maak een screenshot van het resultaat
    - sla deze op onder je M5ProgWebC24 map
        - met de naam `02 appusertest nope.png`


## herstellen van de rechten

- verander de rechten terug naar:
    - select
    - delete
    - insert
    - update
    - execute

## extra:

- pas index.php aan, en select daar alles uit test
- check wat er gebeurt!

## klaar

- commit & push nu alles naar je repository! 
