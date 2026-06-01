# 🐍 Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

---

## 🧠 ALGORITHM

1. **Create Class `A`**:
   - Define the `__init__()` method to initialize the object with a value `a`.

2. **Overload the `<` Operator**:
   - Define the `__lt__()` method with logic:
     - If `self.a < o.a`, return `"ob1 is less than ob2"`
     - Else, return `"ob2 is less than ob1"`

3. **Create Objects**:
   - Instantiate two objects `ob1` and `ob2` with values.

4. **Use `<` Operator**:
   - Use `print(ob1 < ob2)` to trigger the overloaded behavior.

---

## 💻 Program
~~~
class Student:
    def __init__(self, marks):
        self.marks = marks

    # Overloading the < operator
    def __lt__(self, other):
        return self.marks < other.marks

# Example usage
s1 = Student(85)
s2 = Student(92)

if s1 < s2:
    print("Student 1 has fewer marks than Student 2")
else:
    print("Student 1 has more or equal marks than Student 2")
~~~
## Output
~~~
Student 1 has fewer marks than Student 2
~~~
## Result
successfuly created
