# SQLodev6
## sql sorguları patika odev 6 ##
**Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.**<br/>
1.film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?<br/><br/>
SELECT AVG(rental_rate) from film;<br/><br/><br/>
2film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?<br/><br/>
SELECT count(*) from film<br/>
where title LIKE 'C%';<br/><br/><br/>
3.film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?<br/><br/>
SELECT max(length) from film<br/>
where rental_rate=0.99;<br/><br/>
4.film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?<br/><br/>
SELECT  COUNT(DISTINCT(replacement_cost)) from film<br/>
where length>=150;<br/><br/>
