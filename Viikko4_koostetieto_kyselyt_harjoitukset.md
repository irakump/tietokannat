# Viikko 4
# Koostetieto kyselyt harjoitukset

### Kysymys 1
select max(elevation_ft)
from airport;
![image](https://github.com/user-attachments/assets/762affdc-8f2f-453f-a348-939a1c450184)

### Kysymys 2
select continent, count(*)
from country
group by continent;
![image](https://github.com/user-attachments/assets/4105befb-44af-41e3-a406-8698147de82d)

### Kysymys 3
select screen_name, count(*)
from game, goal_reached
where id = game_id
group by screen_name;
![image](https://github.com/user-attachments/assets/497c7b50-f75f-4853-bdc5-23120bb9aa37)

### Kysymys 4
select screen_name
from game
where id in (
select id
from game
where co2_consumed = (select min(co2_consumed) from game) 
);
![image](https://github.com/user-attachments/assets/f8864a5a-7b95-4e17-93c5-5176ec0155ca)

### Kysymys 5


### Kysymys 6


### Kysymys 7


### Kysymys 8


### Kysymys 9


### Kysymys 10

