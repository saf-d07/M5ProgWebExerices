## zomer..

- lees:
    ```
    na de zomer vakantie wil nog wel eens wat kennis zijn weggezakt

    we gaan nu dat even ophalen
    ```

## files


- maak een nieuwe map onder je M5Prog 
    - 03 herhaal les
        - maak een sql file aan om je sql in op te slaan
            - beyondspace.sql

## tabellen

- gebruik de volgende sql:
    > gebruik het workbench sql window!
    ```SQL
   -- Table: Crew
    CREATE TABLE Crew (
        crew_id INT AUTO_INCREMENT PRIMARY KEY,
        name VARCHAR(100),
        species VARCHAR(50),
        `rank` VARCHAR(50),
        birth_year INT
    );

    -- Table: Missions
    CREATE TABLE Missions (
        mission_id INT AUTO_INCREMENT PRIMARY KEY,
        mission_name VARCHAR(100),
        destination VARCHAR(100),
        start_date DATE,
        end_date DATE
    );

    -- Table: Crew_Missions (many-to-many relationship)
    CREATE TABLE Crew_Missions (
        crew_id INT,
        mission_id INT,
        role VARCHAR(50),
        FOREIGN KEY (crew_id) REFERENCES Crew(crew_id),
        FOREIGN KEY (mission_id) REFERENCES Missions(mission_id)
    );


    ```

## zichtbaar?

- zie je de tabellen meteen?
    - zoek uit waarom niet en hoe je dat kan verversen
- waarom staat rank als `rank` terwijl de rest niet zo staat? 

## Bewaar

- zorg dat je de sql voor alle opdrachten hieronder bewaard in de sql file!


## INSERT 

- Voeg 3 bemanningsleden en 2 missies toe.
    > geef zelf id's mee!
    - geef minimaal 1 de soort `Andoriaan`
- zorg dat de Crew_Missions ook gevuld is. 
    - verdeel de crew over 2 missies, en laat sommige bij beide meegaan

## SELECT + WHERE
- Selecteer alle bemanningsleden 
- Selecteer alle bemanningsleden van soort 'Andoriaan' die geboren zijn na het jaar 2300.


## git

commit je script, diagram en screenshot naar je git repository voor de vak!