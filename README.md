Top 5 Countries with the Most Content:

The United States leads by a large margin with 2,818 titles.
India comes second with 972 titles.
The United Kingdom follows with 419 titles.
Japan has 245 titles.
South Korea has 199 titles.

Incomplete Information:

Some rows may have missing values for important columns such as country, date_added, or rating. This incomplete information can skew the analysis or lead to inaccurate conclusions.
Question 2: In which countries are there more than 100 shows with a popularity score above 80?
SELECT country, COUNT(*) AS show_count
FROM tv_shows
WHERE popularity_score > 80
GROUP BY country
HAVING COUNT(*) > 100;
 What are the top 10 most popular shows in the United States?
SELECT show_title, ... (other relevant columns)
FROM tv_shows
WHERE country = 'US'
ORDER BY popularity_score DESC
LIMIT 10;
