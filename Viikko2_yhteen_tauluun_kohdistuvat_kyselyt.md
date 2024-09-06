# Viikko 2
# Yhteen tauluun kohdistuvien kyselyiden harjoitukset

### Kysymys 1
select * from goal;

![image](https://github.com/user-attachments/assets/54dad38d-cddc-4dd8-a722-6d312246d208)

### Kysymys 2
select name, airport.type 
from airport 
where iso_country = "FI";
![image](https://github.com/user-attachments/assets/8c2dcf0e-4167-4795-bb7e-fd0e1e8bbbfe)

### Kysymys 3
select name
from airport
where iso_country = "FI"
order by name asc;
![image](https://github.com/user-attachments/assets/188e1a8c-3378-4efd-826c-b0a0bf077f70)

### Kysymys 4
select name, type
from airport
where iso_country = "FI"
order by type, name;
![image](https://github.com/user-attachments/assets/2af87ffb-abc8-4a6f-a4e7-0cbb53826e91)

### Kysymys 5
select name
from country
where name like "F%";
![image](https://github.com/user-attachments/assets/bea2d520-4c91-4fcf-9576-3000d15df2d6)

### Kysymys 6
select name
from country
where name like "%f%";
![image](https://github.com/user-attachments/assets/59d57db3-0f2e-40ab-9779-a8f08d9d157b)

### Kysymys 7
select location
from game
where screen_name = "Vesa";
![image](https://github.com/user-attachments/assets/e12b7cab-f045-41ab-98ae-b89a27c494e7)

### Kysymys 8
select co2_consumed
from game
where screen_name = "Ilkka";
![image](https://github.com/user-attachments/assets/d8d60b90-c201-4cf0-ac5c-ec011e67d0d5)

### Kysymys 9
select co2_budget
from game
where screen_name = "Ilkka";
![image](https://github.com/user-attachments/assets/31565dae-9de2-42ff-87f1-4eb0396c4bd6)
