# Point of Sale (POS) App

A desktop POS application built with Java Swing and MySQL. Handles staff login, sales entry, stock updates, and supervisor approval workflows — developed as a university final project.

## Features

- Staff login with role-based access (cashier / supervisor)
- Sales entry with per-item and total calculation
- Stock update after each transaction
- Supervisor password confirmation for sensitive operations
- MySQL-backed persistent storage

## Tech Stack

| Tool | Role |
|---|---|
| Java (Swing) | Desktop GUI |
| MySQL | Relational database |
| JDBC | Java ↔ MySQL connectivity |

## Project Structure

```
src/
├── Connect.java      # JDBC connection helper
├── Login.java        # Staff login screen
├── Main.java         # Entry point
├── SalesEntry.java   # Sales transaction UI
├── UpdateStock.java  # Stock management UI
└── User.java         # User model
uasbad.sql            # Database schema and seed data
```

## Setup

1. Install Java 8+ and MySQL.
2. Import `uasbad.sql` into MySQL to create the schema and seed data.
3. In `src/Connect.java`, update the connection string with your local MySQL host, database name, and credentials.
4. Add the MySQL JDBC driver (`mysql-connector-java-*.jar`) to your classpath (not included — download from [dev.mysql.com](https://dev.mysql.com/downloads/connector/j/)).
5. Compile and run `Main.java`.

## Skills demonstrated

- Java Swing GUI layout and event handling
- JDBC database connectivity
- Role-based access control
- SQL DDL/DML for schema design and seeding
