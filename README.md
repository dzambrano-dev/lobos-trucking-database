# Lobos Trucking Database (CLI)

This project is a lightweight command-line database application designed to manage clients, jobs, and invoices for a small trucking operation. It uses SQLite for data storage and Python for a simple administrative interface.

The goal of this project is to demonstrate core systems concepts such as relational database design, data integrity, and safe database interaction through a CLI-based workflow.

---

## Features

- Relational database schema with enforced foreign keys
- Separation of schema definition and sample data
- Command-line interface for basic administrative tasks
- Parameterized SQL queries to prevent SQL injection
- Clear distinction between read and write operations

---

## Database Design

The database consists of three related tables:

- **clients**: stores client contact information
- **jobs**: tracks work performed for each client
- **invoices**: records billing and payment status for completed jobs

Relationships are enforced using foreign keys to ensure referential integrity. Business rules such as one invoice per job and valid job statuses are handled at the database level.

---

## File Structure
  app.py # Command-line interface and application logic
  schema.sql # Database schema and table definitions
  sample_data.sql # Fictional demo data for testing
  README.md

---

## How to Run

1. Ensure Python 3 is installed.
2. From the project directory, run:

```bash
python app.py
