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

Question 6:
    SELECT name FROM city WHERE name LIKE 'F%' LIMIT 25;

Question 7:    
    SELECT COUNT(a.name) FROM city a JOIN country b ON Code=CountryCode WHERE (code='CHN');

Question 8:
    SELECT population FROM country WHERE population > 1 ORDER BY population LIMIT 1;

Question 9:
    SELECT COUNT(name) FROM country;

Question 10;
    SELECT name FROM country ORDER BY SurfaceArea DESC LIMIT 10;

Question 11:
    SELECT a.name FROM city a JOIN country b ON CountryCode=Code WHERE (b.name='Japan') ORDER BY b.Population DESC LIMIT 5;

 Question 12:
    Fix Mistake
         Update country set HeadOfState = 'Elizabeth II' where HeadOfState IN ('Elisabeth II');
            SELECT Name, Code FROM country WHERE HeadOfState='Elizabeth II';

Question 13:
    

Question 14:
    SELECT COUNT(CountryCode), language FROM CountryLanguage GROUP BY language;

Question 15:
    SELECT Name, GNP FROM country ORDER BY GNP DESC LIMIT 10;

Question 16:
    SELECT country.name, COUNT(countrylanguage.Language) FROM countrylanguage JOIN country ON country.Code=countrylanguage.CountryCode ORDER BY countrylanguage.Language DESC LIMIT 10;

Question 17:

Question 18:
    SELECT name FROM country WHERE LifeExpectancy != 0 ORDER BY LifeExpectancy ASC LIMIT 1;

Question 19: 
   SELECT GovernmentForm, COUNT(GovernmentForm) AS Government_Count FROM country GROUP BY GovernmentForm ORDER BY COUNT(GovernmentForm) DESC LIMIT 3;

Question 20:
    SELECT COUNT(name) FROM country WHERE indepyear IS NOT NULL;
