# database-lab — Learn, Practice, and Build with Databases


## ✍️ Author
- **Name**: Shiwoo Min
- **Role**: Full-Stack Developer · DevOps Engineer · Founder of Artiordex  
- **Contact**: artiordex@gmail.com


## 📝 Overview
This repository is a hands-on lab for relational and NoSQL databases. It includes schema design, querying, indexing, transactions, performance tuning, and client tooling. All scripts, sample data, and notes are version-controlled. You can spin up services locally with Docker and connect using DBeaver or DataGrip.


## 🚀 Goals
1. Practice SQL/DDL/DML across multiple engines
2. Compare engine-specific features and SQL dialects
3. Learn indexing, query plans, transactions, isolation levels
4. Explore NoSQL/Key-Value basics with MongoDB/Redis
5. Keep all experiments reproducible via Docker & Git


## ⚙️ Environment
- **OS**: Windows 11 Pro (WSL2 optional)
- **Clients**: DBeaver EE (with Git support), JetBrains DataGrip
- **Runtime**: Docker Desktop + Docker Compose
- **Databases**: Oracle, MySQL, MariaDB, PostgreSQL, MS-SQL, MongoDB, SQLite, Redis


## 🗓 2-Week Learning Plan

#### Week 1 – Database Fundamentals & SQL Basics
1. Environment Setup: Configure Docker Compose for multiple databases (MySQL, PostgreSQL, MongoDB, etc.) and set up client tools (DBeaver/DataGrip)  
2. RDBMS Basics: Understand databases, tables, and schemas / basic DDL commands (CREATE, DROP, ALTER)  
3. Basic SQL Queries: SELECT, WHERE, ORDER BY, LIMIT/OFFSET, DISTINCT  
4. Data Manipulation: INSERT, UPDATE, DELETE / Transactions (COMMIT, ROLLBACK)  
5. Basic Joins: INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL OUTER JOIN  

#### Week 2 – Advanced SQL, NoSQL & Practical Usage
6. Advanced SQL: GROUP BY, HAVING, subqueries, window functions  
7. Data Modeling & Constraints: Primary Keys, Foreign Keys, UNIQUE, CHECK, INDEX design  
8. NoSQL Fundamentals: MongoDB data modeling, CRUD operations, Aggregation Framework  
9. Advanced Features: Stored Procedures, Views, Triggers, Functions  
10. Performance & Optimization: Query execution plans, index tuning, partitioning  
11. Project Practice:  
    - Import public datasets (CSV/JSON)  
    - Compare queries and results across multiple DB engines  
    - Create scripts for backup, restore, and migration 


## 🗃 Folder Structure
```
database-lab/
├─ docker/                  # compose files, init scripts
│  ├─ compose.yml
│  └─ init/
│     ├─ mysql/             # *.sql executed on first start
│     ├─ mariadb/
│     ├─ postgres/
│     ├─ mssql/
│     └─ mongo/             # *.js for mongosh --eval or init scripts
├─ sql/
│  ├─ oracle/
│  ├─ mysql/
│  ├─ mariadb/
│  ├─ postgres/
│  ├─ mssql/
│  ├─ sqlite/
│  └─ common/               # engine-agnostic exercises
├─ data/                    # csv/json sample datasets
├─ notebooks/               # study notes (md)
├─ clients/
│  ├─ dbeaver/              # exported connections, ERD, projects
│  └─ datagrip/             # data sources settings (sanitized)
├─ scripts/                 # helper scripts (seed, backup/restore)
├─ .env.example             # environment variables for compose
└─ README.md
```

## ⏳ Project Duration & Updates
- Date: 2025-08-11 → 2025-08-22
- Updates
```
2025-08-11 - Initial repository setup with folder structure and .env example
2025-08-12 - Added Docker Compose configuration for MySQL, PostgreSQL, and MongoDB
2025-08-13 - Created sample datasets (CSV, JSON) for practice
2025-08-15 - Implemented basic SQL scripts for table creation and data insertion
2025-08-17 - Added JOIN query examples for MySQL and PostgreSQL
2025-08-18 - Integrated MongoDB aggregation examples
2025-08-20 - Added backup and restore helper scripts for multiple databases
2025-08-22 - Completed multi-database mini-project comparing query performance
```

## 📝 Daily Learning Log
```
Template
2025-08-__ (Day __)
- Topics: (Database/Feature)
- Practice: (File/Folder path in sql/, docker/, or scripts/)
- Dataset: (File path in data/)
- Notes:
- References: (Book/Course/Link)
```


## 🧩 Connection Endpoints
| Engine     | Host      | Port  | User     | Password      | DB/Service        |
| ---------- | --------- | ----- | -------- | ------------- | ----------------- |
| PostgreSQL | localhost | 5432  | postgres | postgres      | postgres          |
| MySQL      | localhost | 3306  | root     | root          | mysql             |
| MariaDB    | localhost | 3307  | root     | root          | mysql             |
| MS-SQL     | localhost | 1433  | sa       | P\@ssw0rd!123 | master            |
| MongoDB    | localhost | 27017 | root     | root          | admin             |
| Redis      | localhost | 6379  | -        | -             | 0                 |
| SQLite     | - (file)  | -     | -        | -             | `sql/sqlite/*.db` |


## 📚 References

#### 📖 Books
- [Learning SQL](https://www.oreilly.com/library/view/learning-sql-3rd/9781492057604/)
- [SQL Cookbook](https://www.oreilly.com/library/view/sql-cookbook-2nd/9781492077442/)
- [Database Internals](https://www.oreilly.com/library/view/database-internals/9781492040330/)

#### 🗂 GitHub & Repositories
- [GitHub Topics: learn-sql](https://github.com/topics/learn-sql)
- [GitHub Topics: database](https://github.com/topics/database)

#### 🎓 Online Courses
- [Databases and SQL for Data Science](https://www.coursera.org/learn/sql-data-science)
- [The Complete SQL Bootcamp](https://www.udemy.com/course/the-complete-sql-bootcamp/)
- [Relational Database Design](https://www.edx.org/course/databases-5-sql)

#### 🏛 Official Documentation
- [PostgreSQL Documentation](https://www.postgresql.org/docs/)
- [MySQL Documentation](https://dev.mysql.com/doc/)
- [MariaDB Documentation](https://mariadb.com/kb/en/documentation/)
- [MS-SQL Documentation](https://learn.microsoft.com/sql/)
- [MongoDB Documentation](https://www.mongodb.com/docs/)
- [SQLite Documentation](https://www.sqlite.org/docs.html)
- [Redis Documentation](https://redis.io/docs/)

#### 🛠 Client Tools Documentation
- [DBeaver Official Site](https://dbeaver.io/)
- [DataGrip Official Site](https://www.jetbrains.com/datagrip/)

#### 🌐 Tutorials & Community
- [SQLZoo](https://sqlzoo.net/)
- [Mode SQL Tutorial](https://mode.com/sql-tutorial/)
- [W3Schools SQL Tutorial](https://www.w3schools.com/sql/)
- [Stack Overflow - SQL Tag](https://stackoverflow.com/questions/tagged/sql)
