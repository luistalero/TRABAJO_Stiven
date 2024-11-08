# CONSULTAS JOIN

```sql
-- 1 
SELECT cu.first_name AS customer_first_name, cu.last_name AS customer_last_name, cu.last_update AS last_update
FROM customer AS cu
ORDER BY cu.last_update DESC
LIMIT 20;

-- 2
SELECT f.title AS movie_title, f.release_year AS release_year
FROM film AS f
ORDER BY f.release_year DESC
LIMIT 10;

-- 3 
SELECT p.payment_id AS payment_id, p.amount AS payment_amount, cu.first_name AS customer_first_name, cu.last_name AS customer_last_name
FROM payment AS p
JOIN customer AS cu ON p.customer_id = cu.customer_id
ORDER BY p.amount ASC
LIMIT 30;

-- 4
SELECT f.title AS movie_title, f.rating AS movie_rating
FROM film AS f
ORDER BY f.rating DESC
LIMIT 7;

-- 5 
SELECT f.title AS movie_title, i.inventory_id AS inventory_number
FROM film AS f
JOIN inventory AS i ON f.film_id = i.film_id
ORDER BY i.inventory_id ASC
LIMIT 15;

```
# RESULTADOS

- 1

  ![image](https://github.com/user-attachments/assets/5d5f2d03-552f-4f2d-a2df-da851712565c)

- 2

  ![image](https://github.com/user-attachments/assets/bab800b1-5d63-440f-81fe-506b37bd8491)

- 3

  ![image](https://github.com/user-attachments/assets/83c0fbea-6326-48fe-967e-d63f580aa98d)

- 4

  ![image](https://github.com/user-attachments/assets/1d8575c1-89ab-46c3-96c5-e81508bebe3f)

- 5

  ![image](https://github.com/user-attachments/assets/eea048b5-c4ef-414b-b021-5db2ba4e5226)
