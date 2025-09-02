## .env file

We hebben nu onze `.env_template` en `.env` files. 

## UITLEG Database login

- lees deze uitleg:
```
we gaan in het werkveld en de lessen veel met databases werken

WAT we `NOOIT` willen is je login of wachtwoorden in git zetten
Je gevoelige data mag nooit in welke source control ooit.

Dus onze `.env` file waar echte login data in komt mag dus `NOOIT` in git komen.
Als dat wel gebeurt `MOET` je de data veranderen, dus user/password voor het geval dat.

maar hoe doen we dat?
```

## IGNORE

- VOORDAT je commit, maak je een `.gitignore` file
- in de .gitignore file zet je `.env` 
>![](img/ignore.PNG)
> Tip het is handig om standaard .gitignore files te bewaren en het aan te leren die eerst in je project te zetten voordat je begint

## TEST

>![](img/mapstart.PNG)
- ga in je commandprompt/terminal naar de directory `M5ProgWeb`
    > dus waar `.env` en `.env_template` in staan
- type in: 
    - git add
- type in: 
    - git status

## controleren

- staat `.env` ertussen in je staged files?
    * NEE?: je kan verder
    <br>*`GOED`*: 
    > ![](img/goed.PNG)
    * JA?: repareren
    <br>*`FOUT`*: 
    > ![](img/fout.PNG)



## git

commit naar je git repository voor de vak!