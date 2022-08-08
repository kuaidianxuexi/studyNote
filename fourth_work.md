第一题

```sql
create database thrid_week;
use thrid_week;
show tables;
create table if not exists employees(
emp_no int,
birth_date DATE,
first_name varchar(20),
last_name varchar(20),
gender varchar(1),
hire_date DATE
);
insert into employees values (10001, '1953-09-02','Georgi','Facello','M','1986-06-26'),(10002,'1964-06-02','Bezalel','Simmel','F','1985-11-21'),(10003,'1959-12-03','Parto','Bamford','M','1986-08-28'),(10004,'1954-05-01','Christain','Koblick','M','1986-12-01');
select * from employees;
select * from employees where hire_date in (select max(hire_date) from employees);
```

第二题

```sql
use thrid_week

select 
a.film_id,
a.title
from film a 
left join film_category b on a.film_id = b.film_id 
left join category c on b.category_id = c.category_id
where name is null;
-----------------------------------------------------------------------
select 
a.film_id,
a.title
from film a left join film_category b on a.film_id = b.film_id 
where b.film_id is null;
```

第三题

```sql
select * from employees limit 5, 5;
```

第四题

```sql

create index idx_lastname on actor(last_name);

create unique index uniq_idx_firstname on actor(first_name);
```

第五题

```sql
select id , 
	number,
	rank() over(order by number desc) as t_rank
from passing_number;

```

