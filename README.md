# SQL-Ödev10

1. City tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.
```
SELECT city, country
FROM city
LEFT JOIN country
ON  country.country_id = city.city_id;
```
2. Customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.
```
SELECT payment_id,first_name,last_name 
FROM payment 
RIGHT JOIN customer
ON customer.customer_id = payment.customer_id;
```
3. Customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.
```
SELECT rental_id,first_name,last_name 
FROM rental 
FULL JOIN customer
ON customer.customer_id= rental.customer_id;
```

