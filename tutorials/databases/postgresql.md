# PostgreSQL

PostgreSQL is a powerful, open source object-relational database system that uses and extends the SQL language combined with many features that safely store and scale the most complicated data workloads. 

- [Download PostgreSQL](https://www.postgresql.org/download/)

- [How to use PostgreSQL in Visual Studio Code](https://www.kirenz.com/post/2021-12-22-how-to-use-postgresql-in-visual-studio-code/how-to-use-postgresql-in-visual-studio-code/)


- [How to use PostgreSQL with Jupyter Notebooks in Python](https://www.kirenz.com/post/2021-12-22-how-to-use-postgresql-with-jupyter-notebook-in-python/how-to-use-postgresql-with-jupyter-notebook-in-python/)

- [PostgreSQL and pandas in Python](https://www.kirenz.com/post/2021-12-20-postgresql-and-pandas-in-python/postgresql-and-pandas-in-python/)


---

SQL example:

```sql
-- create table
CREATE TABLE teachers (
    id serial,
    first_name varchar(25),
    last_name varchar(50),
    school varchar(50),
    hire_date date,
    salary numeric
);

-- insert values 
INSERT INTO teachers (first_name, last_name, school, hire_date, salary)
VALUES ('Janet', 'Smith', 'F.D. Roosevelt HS', '2011-10-30', 36200), 
       ('Lee', 'Reynolds', 'F.D. Roosevelt HS', '1993-05-22', 65000),
       ('Samuel', 'Cole', 'Myers Middle School', '2005-08-01', 43500),
       ('Samantha', 'Bush', 'Myers Middle School', '2011-10-30', 36200),
       ('Betty', 'Diaz', 'Myers Middle School', '2005-08-30', 43500),
       ('Kathleen', 'Roush', 'F.D. Roosevelt HS', '2010-10-22',38500 ); 
```