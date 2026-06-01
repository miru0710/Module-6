# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
~~~
class Rectangle:
    # Constructor
    def __init__(self, length, breadth):
        self.__length = length     # private variable
        self.__breadth = breadth   # private variable

    # Setter methods (to set values safely)
    def set_length(self, length):
        if length > 0:
            self.__length = length
        else:
            print("Length must be positive")

    def set_breadth(self, breadth):
        if breadth > 0:
            self.__breadth = breadth
        else:
            print("Breadth must be positive")

    # Getter methods (to access private values)
    def get_length(self):
        return self.__length

    def get_breadth(self):
        return self.__breadth

    # Method to calculate area
    def area(self):
        return self.__length * self.__breadth


# Example usage
rect = Rectangle(10, 5)

print("Length:", rect.get_length())
print("Breadth:", rect.get_breadth())
print("Area:", rect.area())

rect.set_length(15)
rect.set_breadth(8)
print("\nAfter modifying values:")
print("Length:", rect.get_length())
print("Breadth:", rect.get_breadth())
print("Area:", rect.area())
~~~
## Output
~~~
Length: 10
Breadth: 5
Area: 50

After modifying values:
Length: 15
Breadth: 8
Area: 120
~~~
## Result
successfuly created
