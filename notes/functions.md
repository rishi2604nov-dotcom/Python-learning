# Functions in Python

## 1. Defining Functions
```python
def greet(name):
    return "Hello " + name

print(greet("Rishikesh"))
```

---

## 2. Default Parameters
```python
def power(x, y=2):
    return x ** y

print(power(3))   # 9
print(power(3, 3))   # 27
```

---

## 3. Multiple Return Values
```python
def get_stats(numbers):
    return min(numbers), max(numbers), sum(numbers)

print(get_stats([2, 4, 6]))
```

---

## 4. Lambda Functions
```python
square = lambda x: x * x
print(square(5))
```
