# MySQLChallenge

Question 1:
    SELECT first_name, last_name FROM Actors;

Question 2;
    SELECT last_name FROM actor WHERE first_name ='John';

Question 3:
    SELECT first_name, last_name FROM actor WHERE last_name ='Neeson';

Question 4:
    SELECT first_name, last_name FROM actor WHERE (actor_id % 10) = 0';

Question 5:
    Select description FROM film WHERE film_id =100;

Question 6;
    Select title FROM film WHERE rating='R';

Question 7:
    Select title FROM film WHERE rating!='R';

Question 8:
    SELECT title FROM film ORDER BY  length ASC LIMIT 10;

Question 9:
     SELECT title FROM film ORDER BY length DESC;

Question 10;
    SELECT * FROM film WHERE special_features='Deleted Scenes;

Question 11:
    SELECT DISTINCT last_name FROM actor ORDER BY last_name DESC;

Question 12:
SELECT last_name FROM actor GROUP BY last_name HAVING COUNT(last_name) >= 1 ORDER BY last_name DESC;

Question 13



    



13