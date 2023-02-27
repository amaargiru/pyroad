## Databases

Learn the general concepts first, and then the specifics of working with specific database management systems. Try working with SQLite, even if you're planning to switch to PostgreSQL later. SQLite is a very popular database, used in Android, Chromium and dozens of other popular projects. You can use SQLite as a convenient local storage alternative to working with files directly.

By the way, try to briefly return to chapter one, Data Structures, to understand how and why the inner workings of databases are structured.

This also provides yet another door into a "another world". Perhaps you would like to tie your future to databases by becoming a [DBA](https://en.wikipedia.org/wiki/Database_administrator)?

```mermaid
flowchart TD

subgraph Databases
direction LR

Databases_basics -.-> SQL -.-> SQLite -.-> MySQL -.-> PostgreSQL -.-> ORM -.-> Analyze_an_execution_plan

subgraph Databases_basics
direction LR
Relational_model("Relational model")
Transaction(Transaction)
subgraph ACID
Consistency(Consistency)
Isolation(Isolation)
end
Nplusone("N+1 problem")
SQL_injection("SQL injection")
NoSQL(NoSQL)
end

subgraph SQL
direction LR

subgraph DDL
CREATE(CREATE)
ALTER(ALTER)
DROP(DROP)
PRIMARY_KEY("PRIMARY KEY")
FOREIGN_KEY("FOREIGN KEY")
ddlmore("...")
end

subgraph DML
SELECT(SELECT)
INSERT(INSERT)
UPDATE(UPDATE)
DELETE(DELETE)
FROM(FROM)
WHERE(WHERE)
SET(SET)

dmlmore("...")
end

DCL(DCL)
TCL(TCL)
SQL_standard("SQL standard")

end

subgraph SQLite
direction LR
SQLite_benefits("SQLite benefits")
Syntax_Diagrams("Syntax Diagrams")
DB_Browser_for_SQLite("DB Browser for SQLite")
end

subgraph MySQL
direction LR
MySQL_Workbench("MySQL Workbench")
end

subgraph PostgreSQL
direction LR
PostgreSQL_benefits("PostgreSQL benefits")
psql(psql)
pgAdmin(pgAdmin)
PostgreSQL_more("...")
end

subgraph ORM
direction LR
peewee(peewee)
SQLAlchemy(SQLAlchemy)
Django_ORM("Django ORM")
end

Analyze_an_execution_plan("Analyze an execution plan")

end
classDef trainee fill:#6ADA6A, stroke-width:3px
classDef middle fill:#FF9900, stroke-width:3px

class Relational_model trainee;
class Transaction trainee;
class Consistency trainee;
class Isolation trainee;
class CREATE trainee;
class ALTER trainee;
class DROP trainee;
class PRIMARY_KEY trainee;
class FOREIGN_KEY trainee;
class SELECT trainee;
class INSERT trainee;
class UPDATE trainee;
class DELETE trainee;
class FROM trainee;
class WHERE trainee;
class SET trainee;
class SQLite_benefits trainee;
class Syntax_Diagrams trainee;
class PostgreSQL_benefits trainee;
class peewee trainee;

class NoSQL middle;
class SQL_standard middle;
class PostgreSQL_more middle;
class SQLAlchemy middle;
class Django_ORM middle;
class Analyze_an_execution_plan middle;
```
