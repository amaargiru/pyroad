## Базы данных

Изучите сначала общие понятия, а потом специфику работы с конкретными системами управления базами данных. Попробуйте поработать с SQLite, даже если позже вы планируете перейти на PostgreSQL. SQLite является очень популярной БД, используется в Android, Chromium и еще в десятках популярных проектов. Вы же можете использовать SQLite в качестве удобного локального хранилища, как альтернативу прямой работе с файлами.

Попробуйте, кстати, ненадолго вернуться к главе первой, «Структуры данных» и разобраться, как и почему устроены внутренности баз данных.

Здесь, кстати, расположена еще одна дверь в «параллельные миры». Может быть вы захотите связать свое будущее с базами данных, став [DBA](https://en.wikipedia.org/wiki/Database_administrator)?

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
