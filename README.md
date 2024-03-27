# SQL_Assignment_9

## Sorgu Senaryoları

* City ve Country Tablolarını Birleştiren INNER JOIN Sorgusu

```bash
SELECT city.city_id, city.city, country.country_id, country.country
FROM city
INNER JOIN country ON city.country_id = country.country_id;
```

Bu sorgu, city ve country tablolarını city_id sütunu üzerinden birleştirir. Sonuçta, her iki tablodaki tüm sütunları içeren yeni bir tablo oluşur.


* Customer ve Payment Tablolarını Birleştiren INNER JOIN Sorgusu

```bash
SELECT payment.payment_id, customer.first_name, customer.last_name
FROM customer
INNER JOIN payment ON customer.customer_id = payment.customer_id;
```

Bu sorgu, customer ve payment tablolarını customer_id sütunu üzerinden birleştirir. Sonuçta, payment_id, first_name ve last_name sütunlarını içeren yeni bir tablo oluşur.

* Customer ve Rental Tablolarını Birleştiren INNER JOIN Sorgusu


```bash
SELECT rental.rental_id, customer.first_name, customer.last_name
FROM customer
INNER JOIN rental ON customer.customer_id = rental.customer_id;
```

Bu sorgu, customer ve rental tablolarını customer_id sütunu üzerinden birleştirir. Sonuçta, rental_id, first_name ve last_name sütunlarını içeren yeni bir tablo oluşur.

Not: Bu sorgular, dvdrental örnek veri tabanı üzerinde çalıştırıldığında, her sorgu için ayrı bir tablo sonucu elde edersiniz.