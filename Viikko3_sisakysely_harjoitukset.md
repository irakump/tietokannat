# Viikko 3
# Sisäkysely harjoitukset

### Kysymys 1
select name
from country
where iso_country in (
select iso_country
from airport
where name like "Satsuma%");
![image](https://github.com/user-attachments/assets/737a6e04-7c42-4634-9cc0-f9f079747977)

### Kysymys 2
select name
from airport
where iso_country in (
select iso_country
from country
where name = "Monaco");
![image](https://github.com/user-attachments/assets/bd4cfde3-cb34-4366-81cd-818dd830ea53)

### Kysymys 3
select screen_name
from game
where id in (
select game_id
from goal_reached
where goal_id in (
select id
from goal
where name = "CLOUDS"));
![image](https://github.com/user-attachments/assets/afc15d8c-fcf7-429e-ba4e-7936979a4e5f)

### Kysymys 4
select name
from country 
where iso_country not in (
select iso_country
from airport);
![image](https://github.com/user-attachments/assets/d232e01e-49da-4130-93a4-c1dc835a4e15)

### Kysymys 5
select name
from goal
where id not in (
select goal_id
from goal_reached
where goal_id not in (
select id
from game
where screen_name = "Heini")); 
![image](https://github.com/user-attachments/assets/49630956-0877-4103-a2eb-46edc99c80ec)
