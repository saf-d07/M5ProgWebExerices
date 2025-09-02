# docker

- lees:
```
de M4 docker was nog niet veilig dat gaan we aanpassen

de docker was nog niet veilig omdat we nog wachtwoorden hadden staan in files die in git kwamen te staan

EN omdat we een root in onze web map hadden staan, als iemand daar bij komt....
```
- maak een html map aan
- zet source en public in in die html file
- maak daar een .env file aan 
    > LET OP: links is oud rechts is nieuw (wat je moet maken)!
    
    > ![](img/aanpassingen.PNG)


## docker compose aanpassen
- open docker-compose.yml in visual studio code
- verander de volgende dingen
    > LET OP: links is oud rechts is nieuw (wat je moet maken)!
    
    >![](img/dockercompare.PNG)

## .env aanpassen
- open de .env die naast de .env_example staat
- verander de volgende dingen
    > LET OP: links is oud rechts is nieuw (wat je moet maken)!

    >![](img/envedit.PNG)

- pas nu de wachtwoorden aan
    - wel goede wachtwoorden!!
    
## .env_example aanpassen
- open de .env_example file
    - zorg dat die er zo uitziet:
    >![](img/rootexample.PNG)

## html/.env aanpassen


- open de .env die naast in de html directory staat
- kopieer alles uit de .env (naast .env_example) BEHALVE DB_ROOT_PASSWORD
    > rechts is de .html env

    >![](img/htmlenv.PNG)

## html/.env_example aanpassen
- open de html/.env_example file
    - zorg dat die er zo uitziet:

    >![](img/htmlexample.PNG)


## klaar

ga naar de volgende opdacht