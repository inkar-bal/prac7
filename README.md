#PhoneBook App (PostgreSQL + Python)

A simple command-line PhoneBook application built with Python and PostgreSQL.

---

##Features

* Add contacts
* Search contacts
* Update name or phone
* Delete contacts
* Import contacts from CSV

---

## Preview

```
--- PhoneBook ---
1. Show all contacts
2. Add contact
3. Import from CSV
4. Search
5. Update phone
6. Update name
7. Delete by name
8. Delete by phone
0. Exit
```

Example output:

```
[1] Adil - 87001234567
[2] Aruzhan - 87007654321
```

---

## Project Structure

* `config.py` → database config
* `dbase.py` → main program
* `phonebook.csv` → sample data

---

## Setup

1. Install dependencies:

```bash
pip install psycopg2
```

2. Create PostgreSQL database:

```sql
CREATE DATABASE phonebook;
```

3. Update config:

```python
DB_host="localhost"
DB_base="phonebook"
DB_user="postgres"
DB_pass="your_password"
```

4. Run app:

```bash
python dbase.py
```

---

## CSV Format

```
Name,Phone
Adil,87001234567
Aruzhan,87007654321
```

---

## Notes

* Uses `psycopg2` to connect to PostgreSQL
* Prevents duplicate phones
* Case-insensitive search supported

---

## 👨‍💻 Author

Your Name
