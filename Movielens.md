# MySQLChallenge - Movielens

Question 1: 
    SELECT title, release_date FROM movies WHERE Release_date BETWEEN '1989-01-01' AND '1993-01-01' ORDER BY release_date DESC;

Question 2:
    SELECT A.title, MIN(B.rating) FROM movies A
JOIN ratings B ON
A.id=B.movie_id;

Question 3:
    SELECT movies.id, title
FROM movies
JOIN genres_movies ON genres_movies.movie_id=movies.id
JOIN genres ON genres.id=genres_movies.genre_id
JOIN ratings ON ratings.movie_id=movies.id
JOIN users ON users.id=ratings.user_id
JOIN occupations ON occupations.id=users.occupation_id
WHERE genres.name='Sci-Fi'
AND users.age='24'
AND users.gender='m'
AND ratings.rating='5'
AND occupations.name='Student';

Question 4:

Question 5:
    SELECT c.name, COUNT(a.id)
    FROM movies a
    JOIN genres_movies b ON a.id=b.movie_id
    JOIN genres c ON b.genre_id=c.id
    GROUP BY c.name
    ORDER BY COUNT(a.id) ASC;