# Patika.dev-SQL-Task-4
 _tablolara sql4.1.csv şeklindeki başlıklardan ulaşabilirsiniz_

-------

Aşağıdaki sorgu senaryolarını **dvdrental** örnek veri tabanı üzerinden gerçekleştiriniz.

1. **film** tablosunda bulunan **replacement_cost** sütununda bulunan birbirinden farklı değerleri sıralayınız.
2. **film** tablosunda bulunan **replacement_cost** sütununda birbirinden farklı kaç tane veri vardır?
3. **film** tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
4. **country** tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
5. **city** tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?

--------

***Yanıtlar***

1.

```sql
select distinct replacement_cost from film;
```

2.

```sql
select count(distinct replacement_cost) from film;
```

3.

```sql
select count(*) from film
where title like 'T%' and rating = 'G';
```

4.

```sql
select count(*) from country
where country like '_____';
```

5.

```sql
select count(*) from city
where city ilike '%R';
```

