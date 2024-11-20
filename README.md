# Detective-Case

This project investigates a fictional detective case using SQL to analyze and solve the mystery. It involves querying datasets to uncover clues, identify suspects, and piece together the sequence of events. This repository demonstrates techniques such as data cleaning, joining tables, filtering, and aggregating data to draw conclusions.

![image](https://github.com/user-attachments/assets/e1497e54-6e66-4672-8141-e712d75d6f90)

## Case Study
A crime has taken place and the detective needs your help. The detective gave you the crime scene report, but you somehow lost it. You vaguely remember that the crime was a murder that occurred sometime on Jan.15, 2018 and that it took place in SQL City. Start by retrieving the corresponding crime scene report from the police department’s database.
## Data
Follow these steps to solve this challenge:

Download the sql-murder-mystery.db file [here](https://drive.google.com/drive/folders/1SLlSSzIqhu9m4p8HmoJYjn5X_GTYdDsf?usp=share_link)
Visit www.sqliteonline.com
Click on file, then open db and load in the database file you downloaded above
Write your SQL queries to see the different tables and the content

## Tools
SQLiteonline.com

## Entity Relationship Diagram
Since We are analysing with SQL it is best that we know the relationship between our tables.
we can always get that

![image](https://github.com/user-attachments/assets/6a5f2130-319b-4004-b3b5-1792f6c4c33e)

## Analysis
We need to note the some few things;
* Date was on Jan.15, 2018.
* Location was SQL City.
  
#### Firstly checking if the details exist in the database
![image](https://github.com/user-attachments/assets/aaa0d13c-c5e6-4db8-9a23-9fd496d71c58)


since it does i would love to know the description

_Security footage shows that there were 2 witnesses. The first witness lives at the last house on "Northwestern Dr". The second witness, named Annabel, lives somewhere on "Franklin Ave"._

So with this lead i need to get to the two witness 
the first witness

![image](https://github.com/user-attachments/assets/f9e90223-77b5-4260-8660-b2de12cf652c)

the second witness 

![image](https://github.com/user-attachments/assets/a4239af3-3b35-4434-b704-d57cfb774f0d)

##### the next thing i decided to do was to check the witnesses account

![image](https://github.com/user-attachments/assets/8677ee4f-6ff9-4f39-a549-029ee8429d43)

the first witness said

_I heard a gunshot and then saw a man run out. He had a "Get Fit Now Gym" bag. The membership number on the bag started with "48Z". Only gold members have those bags. The man got into a car with a plate that included "H42W"._

Second said:

_I saw the murder happen, and I recognized the killer from my gym when I was working out last week on January the 9th._

Since they were both related to gym i decided to go futher to investigate the first witness account

![image](https://github.com/user-attachments/assets/07652563-34c4-43bf-a6c9-daca12ad4bdb)

we are getting close to knowing who the murderer is but we can't just nail him based on one witness when we have two let's confirm if it mattches the other witness report

![image](https://github.com/user-attachments/assets/236ba7ca-4488-4327-8265-d929ec271c09)


so i need to check if the two witnessess account matches

![image](https://github.com/user-attachments/assets/27e92993-9b80-4a05-9824-0e33d1a9b680)

so finally we can say the killer if _**Jeremy Bowers**_

Never imagined this. He was already interviewed and he confessed to the Murder

![image](https://github.com/user-attachments/assets/f08c8ff5-33c1-4a9a-b0b7-99f1abf49a3a)

Saying 
_I was hired by a woman with a lot of money. I don't know her name but I know she's around 5'5" (65") or 5'7" (67"). She has red hair and she drives a Tesla Model S. I know that she attended the SQL Symphony Concert 3 times in December 2017.
_

so we need to get the woman that hired Jeremy .

![image](https://github.com/user-attachments/assets/770f1581-47f5-48b0-9776-321ac57b9a64)


While we already know the killer we now get to know the person that hired him was _**Miranda Priestly**_

and according to jeremy i decided to go futher to check hoe rich she was and lo and behold she was part of the top 50 Richest in SQL City to be precise she is the 47 richest person in the city.
