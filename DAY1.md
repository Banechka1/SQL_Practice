# DAY1
### TASK2
---
```
SELECT name, age FROM person WHERE address = 'Moscow';
```
![DAY1_2](https://github.com/Banechka1/SQL_Practice/assets/108561676/963000b4-9fe7-4d2a-ae3d-2e2eed5f502e)
---

### TASK3
---
```
SELECT name, age FROM person WHERE gender = 'female' AND address = 'Kazan' ORDER BY name;
```
![image](https://github.com/Banechka1/SQL_Practice/assets/108561676/207a8941-ff40-4a17-b2b7-0f26c67591ea)

---

### TASK4
---
```
SELECT * FROM pizzeria WHERE rating >= 3.5 AND rating <= 5
UNION ALLSELECT * FROM pizzeria WHERE rating BETWEEN 3.5 AND 5 ORDER BY rating;
```
![image](https://github.com/Banechka1/SQL_Practice/assets/108561676/cb56e808-e1a6-4c98-86d7-a3d3d39cfccb)

---

### TASK5
---
```
SELECT person_id FROM person_visits WHERE pizzeria_id = 2 OR visit_date BETWEEN '2022-01-01' AND '2022-01-04' ORDER BY person_id DESC
```
![image](https://github.com/Banechka1/SQL_Practice/assets/108561676/4339a11e-7827-4d5d-866c-d6c8a5c3107f)

---

### TASK6
---
```
SELECT name FROM person WHERE id IN (
SELECT person_id FROM person_order)
```
![image](https://github.com/Banechka1/SQL_Practice/assets/108561676/82d1b2b2-f471-49dd-943f-3ab2dd8f0e71)

---

### TASK7
---
```
SELECT EXISTS(SELECT 1 FROM person WHERE name = 'Anna') as result;
```
![image](https://github.com/Banechka1/SQL_Practice/assets/108561676/bd618ea2-3012-4f66-a6c9-26a14eec8477)

---
