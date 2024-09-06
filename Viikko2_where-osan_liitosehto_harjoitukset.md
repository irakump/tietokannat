# Viikko 2
# Where-osan liitosehto harjoitukset

### Kysymys 1
select country.name as "country name", airport.name as "airport name"
from airport, country
where airport.iso_country = country.iso_country 
and country.name = "Iceland";
![image](https://github.com/user-attachments/assets/8cd23e21-9e04-4d99-bb80-53160afa096e)

### Kysymys 2
select airport.name as "airport name"
from airport, country
where airport.iso_country = country.iso_country
and type = "large_airport"
and country.name = "France";
![image](https://github.com/user-attachments/assets/90cb98d8-f964-4196-80c7-a28c753b3b13)

### Kysymys 3
select country.name as country_name, airport.name as airport_name
from airport, country
where airport.iso_country = country.iso_country
and country.continent = "AN";
![image](https://github.com/user-attachments/assets/8be5cba6-b251-4d5f-bb51-55322829b9bd)

### Kysymys 4
select elevation_ft
from airport, game
where location = ident
and screen_name = "Heini";
![image](https://github.com/user-attachments/assets/00138bce-e08f-4d37-a727-cb7e432c4597)

### Kysymys 5
select elevation_ft * 0.3048 as elevation_m
from airport, game
where location = ident
and screen_name = "Heini";
![image](https://github.com/user-attachments/assets/e11628e7-c524-4be4-b5e3-985442a3e480)

### Kysymys 6
select airport.name
from airport, game
where location = ident
and screen_name = "Ilkka";
![image](https://github.com/user-attachments/assets/34af31dc-5661-48d5-a64d-24da9f4dc430)

### Kysymys 7
select country.name
from airport, country, game
where location = ident
and airport.iso_country = country.iso_country
and screen_name = "Ilkka";
![image](https://github.com/user-attachments/assets/c116d353-5ecc-4c5f-8754-b611a381baa2)

### Kysymys 8
select goal.name
from goal, goal_reached, game
where goal.id = goal_id
and game_id = game.id
and screen_name = "Heini";
![image](https://github.com/user-attachments/assets/a6d25fe6-edeb-4915-8c2c-0c97ac542b50)

### Kysymys 9
select airport.name
from airport, goal, game, goal_reached
where goal.id = goal_id
and game_id = game.id
and ident = location
and screen_name = "Ilkka"
and goal.name = "CLOUDS";
![image](https://github.com/user-attachments/assets/c45458ff-78e2-4efa-bd0b-2c8b2aee29f3)

### Kysymys 10
select country.name
from airport, goal, game, goal_reached, country
where goal.id = goal_id
and game_id = game.id
and ident = location
and airport.iso_country = country.iso_country
and screen_name = "Ilkka"
and goal.name = "CLOUDS";
![image](https://github.com/user-attachments/assets/dc9ae000-df26-4e7b-b883-d79a48b29b6d)
