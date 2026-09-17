# SmartBank – Bank Management System

A desktop Bank Management System built with **Java Swing** and **MySQL**. It provides separate dashboards for **Clients**, **Managers**, and **Accountants**, supporting account creation, deposits/withdrawals, transfers, cheque deposits, cardless withdrawal, and PDF e-statement generation.

## Tech Stack
- Java (Swing)
- MySQL + JDBC
- iText (PDF generation)

## How to Run

1. **Set up the database**
   - Install MySQL and start the server.
   - Open MySQL Workbench (or CLI) and run `MySQL Script.sql` — this creates the `bank_schema` database, tables, and sample data.

2. **Configure the connection**
   - Open `BM_System/src/def_pkg/DB_Handler.java`.
   - Update the `url`, `username`, and `password` fields to match your MySQL setup (default expects MySQL running on `localhost:3307`).

3. **Add the libraries**
   - In your IDE (e.g. Eclipse/IntelliJ), add all `.jar` files from `BM_System/libs/` to the project's build path.

4. **Run the app**
   - Open the project in your IDE.
   - Run `BM_System.java` (the main class in `def_pkg`).
   - The login screen will launch — use the sample credentials from `MySQL Script.sql` (e.g. `rajesh55` / manager, `danielt211` / accountant, or a client login) to sign in.

## Project Structure
```
BM_System/
├── libs/        → external JARs (MySQL connector, iText, etc.)
└── src/def_pkg/ → Java source files (GUI, DB handler, models)
MySQL Script.sql → database schema + sample data
```
