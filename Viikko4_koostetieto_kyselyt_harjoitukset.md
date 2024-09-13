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
select country.name, count(*)
from airport
inner join country on airport.iso_country = country.iso_country
group by country.name
order by count(*) desc
limit 50;
![image](https://github.com/user-attachments/assets/7ac2c1ec-9c5f-4624-ad8b-92e5021f085f)

### Kysymys 6
select country.name
from country
inner join airport on airport.iso_country = country.iso_country
group by country.iso_country
having count(*) > 1000;
![image](https://github.com/user-attachments/assets/6d0261c2-b1f1-412d-ac53-cf4090e314bb)

### Kysymys 7
select name 
from airport
where elevation_ft = (select max(elevation_ft) from airport
);
![image](https://github.com/user-attachments/assets/8a786817-222b-466b-b987-82501900a020)

### Kysymys 8
select country.name
from country
inner join airport on airport.iso_country = country.iso_country
where elevation_ft = (select max(elevation_ft) from airport);
![image](https://github.com/user-attachments/assets/6bdd0599-519f-425f-ab16-231145bf4ca8)

### Kysymys 9
select count(*)
from goal_reached
inner join game on game_id = id
where screen_name = "Vesa"
group by screen_name;
![image](https://github.com/user-attachments/assets/cccba694-5a2b-4685-b404-6064f02b854d)

### Kysymys 10
select name
from airport
where latitude_deg = (select min(latitude_deg) from airport);
![image](https://github.com/user-attachments/assets/13d9fd45-4cd2-419e-a9d2-c1c6970e24ba)
