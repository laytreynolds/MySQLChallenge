# MySQLChallenge - World

Question 1: 
    SELECT COUNT(name) FROM city WHERE CountryCode='USA';

Question 2: 
    SELECT Population, LifeExpectancy FROM country WHERE Name='Argentina';

Question 3: 
    SELECT Name FROM country WHERE LifeExpectancy IS NOT NULL ORDER BY LifeExpectancy DESC LIMIT 1;

Question 4: 
    SELECT a.name FROM city a JOIN country b ON ID=Capital WHERE (b.name='Spain');

Question 5:
    SELECT a.language FROM CountryLanguage a JOIN Country b ON Code=Countrycode WHERE (b.region='Southeast Asia');




 Question 12:

 Fix Mistake - Update country set HeadOfState = 'Elizabeth II' where HeadOfState IN ('Elisabeth II');

