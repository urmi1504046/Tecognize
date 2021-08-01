# Class2

# What is object-oriented programming?

Object-oriented programming combines a group of variables (properties) and functions (methods) into a unit called an "object." 
These objects are organized into classes where individual objects can be grouped together. OOP can help you consider objects in
a program's code and the different actions that could happen in relation to the objects.

Now let's clear some concepts:

## 1) What is Class?
The class is one of the Basic concepts of OOPs which is a group of similar entities. It is only a logical component and not the physical entity. 
Lets understand this one of the OOPs Concepts with example, if you had a class called “Expensive Cars” it could have objects like Mercedes, BMW,
Toyota, etc. Its properties(data) can be price or speed of these cars. While the methods may be performed with these cars are driving, reverse, braking etc.

Following code defines a class.

   class ClassName {

    //attributes
    //methods
         };

**Class Properties**
 * Attributes
 * Methods
 * Constructor
 
 **Attributes:** Class attributes are just variables from a general programming point of view. But when it comes to Object Oriented Programming, these class attributes define the state of the class objects.

Following class defines a class named Student, with three attributes.

  class Student {
    string name;
     int id;
     int section;
     };

**Methods:** Methods of a class defines the behavior of the class objects. Class methods are functions that can be accessed within the class or on the class objects.

Following example, defines a class named Student with method printDetails()

    
    class Student {
   
      //attributes
          string name;
          int id;
          int section;
 
    //methods
    void printDetails(){
      cout << "Name : " << name << endl;
      cout << "id : " << name << endl;
      cout << "Section : " << name << endl;
      }
      };

 
 
## 2) What is a constructor?
A constructor is a special type of method that has the same name as the class and is used to initialize objects of that class.

def__init__(self,....)

## 3) What is Object?
An object can be defined as an instance of a class, and there can be multiple instances of a class in a program. An Object is one of the Java OOPs 
concepts which contains both the data and the function, which operates on the data. For example - chair, bike, marker, pen, table, car, etc.

To create a class object, you have to declare a variable with the class type, just like you declare an integer with variable name and int datatype.

In the following, example, we shall define a class named Student and create an object for this class in the main method.
  class Student {
    public:
     string name;
     int id;
     int section;
 
    public:
    void printDetails(){
       cout << "Name : " << name << endl;
       cout << "id : " << name << endl;
       cout << "Section : " << name << endl;
    }
  };
 
   int main() {
    //create class object
    Student student_1;
  }
An object with variable name **student_1** of type Student has been created.

## 4) What is the difference between a class and a structure?
**Class:** User-defined blueprint from which objects are created. It consists of methods or set of instructions that are to be performed on the objects.

**Structure:** A structure is basically a user-defined collection of variables which are of different data types.

## 5) What is the difference between a class and an object?
 

Object | Class
-------|-------
A real-world entity which is an instance of a class |	A class is basically a template or a blueprint within which objects can be created
An object acts like a variable of the class	| Binds methods and data together into a single unit
An object is a physical entity | A class is a logical entity
Objects take memory space when they are created |	A class does not take memory space when created
Objects can be declared as and when required	| Classes are declared just once

## 6) Differentiate between a class and a method.
Class |	Method
------|-------
A class is basically a template that binds the code and data together into a single unit. Classes consist of methods, variables, etc | Callable set of instructions also called a procedure or function that are to be performed on the given data


## 7) What are the four basics of object-oriented programming?
Object-oriented programming has four basic concepts: encapsulation, abstraction, inheritance and polymorphism. Even if these concepts seem incredibly complex,
understanding the general framework of how they work will help you understand the basics of a computer program. Here are the four basic theories and what they entail:

* Encapsulation
* Abstraction
* Inheritance
* Polymorphism

### Encapsulation
The different objects inside of each program will try to communicate with each other automatically. If a programmer wants to stop objects from interacting with each other,
they need to be encapsulated in individual classes. Through the process of encapsulation, classes cannot change or interact with the specific variables and functions of an object.

### Abstraction
Abstraction is like an extension of encapsulation because it hides certain properties and methods from the outside code to make the interface of the objects simpler. Programmers use abstraction for several beneficial reasons. Overall, abstraction helps isolate the impact of changes made to the code so that if something goes wrong, the change will only affect the variables shown and not the outside code.

### Inheritance
Using this concept, programmers can extend the functionality of the code's existing classes to eliminate repetitive code. For instance, elements of HTML code that include a text box, select field and checkbox have certain properties in common with specific methods.
The main object is the superclass and all objects that follow it are subclasses. Subclasses can have separate elements while adding what they need from the superclass.

### Polymorphism
This technique meaning "many forms or shapes" allows programmers to render multiple HTML elements depending on the type of object. This concept allows programmers to redefine the way something works by changing how it is done or by changing the parts in which it is done. Terms of polymorphism are called overriding and overloading.


# Mutable and Immutable in Python 

An object whose internal state can be changed is mutable. On the other hand, immutable doesn’t allow any change in the object once it has been created.

## Mutable Definition
Mutable is when something is changeable or has the ability to change. In Python, ‘mutable’ is the ability of objects to change their values. These are often the objects that store a collection of data.

## Immutable Definition
Immutable is the when no change is possible over time. In Python, if the value of an object cannot be changed over time, then it is known as immutable. Once created, the value of these objects is permanent.

## List of Mutable and Immutable objects

Objects of built-in type that are mutable are:

* Lists
* Sets
* Dictionaries
* User-Defined Classes (It purely depends upon the user to define the characteristics) 

Objects of built-in type that are immutable are:

* Numbers (Integer, Rational, Float, Decimal, Complex & Booleans)
* Strings
* Tuples
* Frozen Sets
* User-Defined Classes (It purely depends upon the user to define the characteristics)

## Mutable Objects in Python
I believe, rather than diving deep into the theory aspects of mutable and immutable in Python, a simple code would be the best way to depict what it means in Python. Hence, let us discuss the below code step-by-step:

**Creating a list which contains name of Indian cities**  

cities = [‘Delhi’, ‘Mumbai’, ‘Kolkata’]

**Printing the elements from the list cities, separated by a comma & space**

  for city in cities:
		print(city, end=’, ’)

**Output [1]:** Delhi, Mumbai, Kolkata

**Adding a new city to the list cities**

cities.append(‘Chennai’)

**Printing the elements from the list cities, separated by a comma & space** 

for city in cities:
	print(city, end=’, ’)

**Output [2]:** Delhi, Mumbai, Kolkata, Chennai

The above example shows us that we were able to change the internal state of the object ‘cities’ by adding one more city ‘Chennai’ to it, yet, the memory address of the object did not change. This confirms that we did not create a new object, rather, the same object was changed or mutated. Hence, we can say that the object which is a type of list with reference variable name ‘cities’ is a MUTABLE OBJECT.

Let us now discuss the term IMMUTABLE. Considering that we understood what mutable stands for, it is obvious that the definition of immutable will have ‘NOT’ included in it. Here is the simplest definition of immutable– An object whose internal state can NOT be changed is IMMUTABLE. 

**Creating a Tuple with variable name ‘num’**

num = (1, 2)
#Changing the index[0] value from 1 to 3

num[0] = 3
	
TypeError: 'tuple' object does not support item assignment 
Immutable Objects in Python
Once again, a simple code would be the best way to depict what immutable stands for. Hence, let us discuss the below code step-by-step:

**Creating a Tuple which contains English name of weekdays**

weekdays = ‘Sunday’, ‘Monday’, ‘Tuesday’, ‘Wednesday’, ‘Thursday’, ‘Friday’, ‘Saturday’
**Printing the elements of tuple weekdays**

print(weekdays)

Output [1]:  (‘Sunday’, ‘Monday’, ‘Tuesday’, ‘Wednesday’, ‘Thursday’, ‘Friday’, ‘Saturday’)

**uples are immutable, so you cannot add new elements, hence, using merge of tuples with the # + operator to add a new imaginary day in the tuple ‘weekdays’**

weekdays  +=  ‘Pythonday’,

**Printing the elements of tuple weekdays**

print(weekdays)

Output [2]: (‘Sunday’, ‘Monday’, ‘Tuesday’, ‘Wednesday’, ‘Thursday’, ‘Friday’, ‘Saturday’, ‘Pythonday’)

This above example shows that we were able to use the same variable name that is referencing an object which is a type of tuple with seven elements in it. However, the ID or the memory location of the old & new tuple is not the same. We were not able to change the internal state of the object ‘weekdays’. The Python program manager created a new object in the memory address and the variable name ‘weekdays’ started referencing the new object with eight elements in it.  Hence, we can say that the object which is a type of tuple with reference variable name ‘weekdays’ is an IMMUTABLE OBJECT.

### Are strings mutable in Python?
Strings are not mutable in Python. Strings are a immutable data types which means that its value cannot be updated.

### Are lists mutable in Python?
Lists in Python are mutable data types as the elements of the list can be modified, individual elements can be replaced, and the order of elements can be changed even after the list has been created.

### Why are tuples called immutable types?
Tuple and list data structures are very similar, but one big difference between the data types is that lists are mutable, whereas tuples are immutable. The reason for the tuple’s immutability is that once the elements are added to the tuple and the tuple has been created; it remains unchanged.

A programmer would always prefer building a code that can be reused instead of making the whole data object again. Still, even though tuples are immutable, like lists, they can contain any Python object, including mutable objects.










