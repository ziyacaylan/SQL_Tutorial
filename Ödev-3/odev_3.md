# ÖDEV 3

---

1- country tablosunda bulunan country sütunundaki ülke isimlerinden 'A' karakteri ile başlayıp 'a' karakteri ile sonlananları sıralayınız.

```
select country from country where country like 'A%a';
```

2- country tablosunda bulunan country sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.

```
select country from country where LENGTH(country) >= 6 and country like '%n'
```

3- film tablosunda bulunan title sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız.

```
select title from film where lower(title) ilike '%t%t%t%t%';
```

4- film tablosunda bulunan tüm sütunlardaki verilerden title 'C' karakteri ile başlayan ve uzunluğu (length) 90 dan büyük olan ve rental_rate 2.99 olan verileri sıralayınız.

```
select * from film where title like 'C%' and length(title) > 90 and rental_rate = 2.99;
```

@https://academy.patika.dev teşekkürler...

---
