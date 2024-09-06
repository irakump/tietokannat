# Viikko 3
# Join harjoitukset

### Kysymys 1
select country.name as "country name", airport.name as "airport name"
from airport 
inner join country on airport.iso_country = country.iso_country
where country.name = "Finland"
and scheduled_service = "yes";
![image](https://github.com/user-attachments/assets/5bd6a907-be61-43a4-b186-f1e56ad2eb2f)

### Kysymys 2
select screen_name, airport.name as name
from game
inner join airport on location = ident;
![image](https://github.com/user-attachments/assets/9bbabd74-04e6-435e-b557-6175f6eb598f)

### Kysymys 3
select screen_name, country.name
from game
inner join airport on location = ident
inner join country on airport.iso_country = country.iso_country;
![image](https://github.com/user-attachments/assets/54633beb-7022-4fb3-adf9-dd06c2ff92c1)

### Kysymys 4
select airport.name, screen_name
from airport
left join game on location = ident
where airport.name like "%hels%";
![image](https://github.com/user-attachments/assets/606f5821-634c-4fae-9d20-ba97fa9c6ef9)

### Kysymys 5
select name, screen_name
from goal
left join goal_reached ON goal.id = goal_id
left join game on game_id = game.id;
![image](https://github.com/user-attachments/assets/973a93c5-f93d-40e6-ba0b-f91c2a334529)
