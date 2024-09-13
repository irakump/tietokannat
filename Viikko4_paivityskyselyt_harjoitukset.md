# Viikko 4
# Päivityskyselyt harjoitukset

### Kysymys 1
update game
set location = 
(select ident from airport where name = "Nottingham Airport"),
co2_consumed = (co2_consumed + 500)
where screen_name = "Vesa";
![image](https://github.com/user-attachments/assets/2df2599b-fb34-4e0a-abc4-39e620d6c044)

### Kysymys 2
b. goal_reached

### Kysymys 3
delete from goal_reached;
![image](https://github.com/user-attachments/assets/b2ff58b4-e0be-406c-9ddd-a6cfcfb3e543)

### Kysymys 4
delete from game;
![image](https://github.com/user-attachments/assets/b0d80cfe-a8f8-41ca-af64-f2e92de7aab2)
