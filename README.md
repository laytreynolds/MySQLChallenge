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
    SELECT last_name FROM actor GROUP BY last_name HAVING COUNT(last_name) <= 1 ORDER BY last_name DESC;

Question 12:
SELECT last_name FROM actor GROUP BY last_name HAVING COUNT(last_name) >= 1 ORDER BY last_name DESC;

Question 13:
    SELECT actor.first_name, actor.last_name
FROM actor
LEFT JOIN film_actor on actor.actor_id = film_actor.actor_id
GROUP BY actor.actor_id, actor.FIRST_NAME, actor.LAST_NAME
ORDER BY COUNT(*) DESC
LIMIT 1;

Question 14: 

Question 16:
    SELECT AVG(length), category FROM film_list GROUP BY category ORDER BY category ASC;

Question 17:
    SELECT title FROM film WHERE description LIKE '%robot%';

Question 18:
    SELECT COUNT(release_year) FROM film WHERE release_year LIKE 2010;

Question 19:
    SELECT COUNT(release_year) FROM film WHERE release_year LIKE 2010;

Question 20:
    SELECT first_name, last_name FROM staff WHERE staff_id = 2;
