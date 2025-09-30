# Files and Input/Output in Python

## 1. Reading a File
```python
with open("data.txt", "r") as f:
    content = f.read()
    print(content)
```

---

## 2. Writing to a File
```python
with open("output.txt", "w") as f:
    f.write("Hello, file!")
```

---

## 3. Reading Line by Line
```python
with open("data.txt", "r") as f:
    for line in f:
        print(line.strip())
```
