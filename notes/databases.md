# Databases in Python

## 1. Connecting to SQLite
```python
import sqlite3

conn = sqlite3.connect("mydb.db")
cursor = conn.cursor()
```

---

## 2. Creating a Table
```python
cursor.execute("""
CREATE TABLE IF NOT EXISTS users (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    name TEXT,
    age INTEGER
)
""")
conn.commit()
```

---

## 3. Inserting Data
```python
cursor.execute("INSERT INTO users (name, age) VALUES (?, ?)", ("Rishikesh", 28))
conn.commit()
```

---

## 4. Querying Data
```python
cursor.execute("SELECT * FROM users")
rows = cursor.fetchall()

for row in rows:
    print(row)
```

---

## 5. Closing the Connection
```python
conn.close()
```
