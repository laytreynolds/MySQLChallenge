# MySQLChallenge - Saskilla 

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
    SELECT release_year FROM film WHERE title='Academy Dinosaur';

Question 15:
    SELECT AVG(length) FROM film_list;

Question 16:
    SELECT AVG(length), category FROM film_list GROUP BY category ORDER BY category ASC;

Question 17:
    SELECT title FROM film WHERE description LIKE '%robot%';

Question 18:
    SELECT COUNT(release_year) FROM film WHERE release_year LIKE 2010;

Question 19:
    SELECT title FROM film_list WHERE category LIKE 'horror';

Question 20:
    SELECT first_name, last_name FROM staff WHERE staff_id = 2;

Question 21:
    SELECT A.title FROM film A
INNER JOIN film_actor B ON A.film_id=B.film_id
INNER JOIN actor C ON B.actor_id=C.actor_id
WHERE (C.first_name='Fred' AND C.last_name='Costner');


Question 22:
    SELECT DISTINCT COUNT(country) FROM country;

Question 23:
    SELECT name FROM language ORDER BY name DESC;

Question 24:
    SELECT first_name, last_name FROM actor WHERE last_name LIKE'%son' ORDER BY first_name ASC;

Question 25:
     SELECT COUNT(title), category FROM film_list GROUP BY category ORDER BY COUNT(title) DESC LIMIT 1;
   





