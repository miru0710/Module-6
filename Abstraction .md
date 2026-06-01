# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
~~~
from abc import ABC
class type_shape(ABC): 
  def area(self):
    #create abstract method area()
    pass

class Rectangle(type_shape):
  length = 6
  breadth = 4
  def area(self):
    return self.length * self.breadth

class Circle(type_shape):
  radius = 7
  #define area function to calculate area
  def area(self):
      return 3.14*self.radius**2
class Square(type_shape):
  length = 4
  #define area function to calculate area
  def area(self):
      return self.length**2

class triangle:
  length = 5
  width = 4
  #define area function to calculate area
  def area(self):
      return (self.length*self.width)/2
r = Rectangle() # object created for the class 'Rectangle'
c = Circle() # object created for the class 'Circle'
s = Square() # object created for the class 'Square'
t = triangle() # object created for the class 'triangle'
print("Area of a rectangle:", r.area()) # call to 'area' method defined inside the class.
print("Area of a circle:", c.area()) # call to 'area' method defined inside the class.
print("Area of a square:", s.area()) # call to 'area' method defined inside the class.
print("Area of a triangle:", t.area()) # call to 'area' method defined inside the class.
~~~
## Output
<img width="796" height="378" alt="image" src="https://github.com/user-attachments/assets/f08a79e5-be44-43c4-8c91-30347a4f00fa" />

## Result
successfuly created
