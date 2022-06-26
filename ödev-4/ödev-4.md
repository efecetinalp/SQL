## SQL ÖDEV - 4

1. Film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.

    ```SQL
    SELECT DISTINCT replacement_cost FROM film;
    ```

2. Film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?

    ```SQL
    SELECT COUNT (DISTINCT replacement_cost) FROM film;
    ```

3. Film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?

    ```SQL
    SELECT COUNT (*) FROM film
    WHERE title LIKE 'T%' AND rating = 'G';
    ```

4. Country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?

    ```SQL
    SELECT COUNT (*) FROM country
    WHERE country LIKE '_____';
    ```

5. City tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?

    ```SQL
    SELECT COUNT (*) FROM city
    WHERE city ILIKE '%r';
    ```