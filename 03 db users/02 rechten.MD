
## admin & schema privileges


- lees deze uitleg:
```
* wij willen nu de rechten geven aan deze gebruiker op ons nieuwe schema `usertest`
* we zitten niet aan de administrative roles tab!! dat is globaal over de hele database en dus `gevaarlijk`
```

#### refresh
- doe het user scherm weer dicht
> ![](img/veelpriv.PNG)
- open daarna het scherm weer (soms laat workbench de users niet meteen zien)
>![](img/users.PNG)


#### privileges aanpassen

- click op de `schema privileges` tab
> ![](img/newuser.PNG)
- hier staat een `Add Entry ...` knop click daarop
- in de popup selecteren we `Alleen` ons schema
> ![](img/selschema.PNG)

- lees deze uitleg:
```
* dit is omdat deze user alleen voor `1 app` is en dus geen rechten nodig heeft op de database of andere schemas. Dit is het `least privilidge` principe: alleen wat je minimaal nodig hebt niets meer

```
## rechten 
- Vink in `object rights` alleen `select`
- meer hebben we niet nodig, maar gebruikelijk voor een app is:
    - select
    - delete
    - insert
    - update
    - execute
- lees deze uitleg:
```
* mogelijk dat je dus voor 1 app meerdere users hebt, afhankelijk van de rollen binnen de app bv:
* een admin rol mag insert & delete
* een lees rol mag alleen select
```

## testen

- start je m5progdock container opnieuw op
- open de index.php
> ![](img/werkt.PNG)
