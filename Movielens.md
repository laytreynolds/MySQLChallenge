# MySQLChallenge - Movielens

Question 1: 
    SELECT title, release_date FROM movies WHERE Release_date BETWEEN '1989-01-01' AND '1993-01-01' ORDER BY release_date DESC;

Question 2:
    SELECT A.title, MIN(B.rating) FROM movies A
JOIN ratings B ON
A.id=B.movie_id;

Question 3:   
            
