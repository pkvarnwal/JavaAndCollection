# Important topics on Java.

* ### [Inheritance](https://github.com/pkvarnwal/JavaAndCollection#inheritance-1)

* ### [Polymorphism](https://github.com/pkvarnwal/JavaAndCollection#polymorphism-1)
* ### [Interface](https://github.com/pkvarnwal/JavaAndCollection#interface-1)

* ### [Abstract](https://github.com/pkvarnwal/JavaAndCollection/blob/master/README.md#abstract)
* ### Interface Implementation
* ### Nested Interface
* ### Interface Variable
* ### Marker Interface
* ### Spannable Interface
* ### Interface vs Inheritance
* ### Functional Interface

* ### Inheritance: 
This is one way of achieving both polymorphism and code reuse at the same time.
Inheritance is when a `class` derives from an existing `class`.

Java does not support cyclic `Inheritance`.
Ex: class A extends class A

* class extends class
* interface extends interface
* class implements interface

### Valid:

* class A extends class B
* class A implements inf1
* class A implements inf1, inf2
* interface inf1 extends inf2
* interface inf1 extends inf2, inf3
* class A extends B implements inf1, inf2

### Invalid:

* class A extends B,C
* class A extends class A
* interface inf1 extends A
* interface inf1 extends inf1
* class A implements inf1, inf2 extends B
* [EXTENDS KEYWORD MUST BE FIRST KEYWORD]

* ### Polymorphism: 
The ability to treat objects of different types in a similar manner.
Ex: Rabbit and tortoise both are animals, and animals can `Move`. 
If you have an instance of an `Animal` then you can call `Move` without knowing which type of animal it is.


* ### Interface:

* If we don't know anything about implementation, just we have requirement specification.
Then we should go for interface.
* Inside interface every method is always public and abstract wether we are declaring or not.
Hence interface is also considered as 100% pure abstract class.
* We can't declare interface method with the following modifiers:
public -> private, protected
Abstract -> final, static, synchronized, native, strictfp.
* Every variable present inside interface is always public, static and final wether we are declaring or not.
* We can't declare interface variable with the following modifiers:
* private, protected, transient, volatile.
* For Interface variables compulsory we should perform initialization at the time of declaration otherwise we will get compile time error.
* Inside interface we can't declare intance and static blocks otherwise we will get compile time error.
* Inside interface we can't declare constructors.
* Interface is able to hold implementation of class of object also.


* ### Functional Interface:

* A functional interface has exactly one abstract method.
* A Comparable interface with a single method 'compareTo' is used for comparison purpose. Java8 has defined a lot of functional interaces 
  to be used extensively in lambda expressions.

* ### Keywords/assert:

* assert is java keyword used to define as `assert statement`. as assert statement is used to declare an expected boolean condition
  in a program. If the program is running with assertions enabled, then the condition is checked at runtime. If the condition is false,
  the java runtime system throws an AssertionError.
  Ex: Assertions may be declared using the following syntax:
  `assert expression1 [: expression2];`
  expression1 is a boolean that will throw the assertion if it is false. When it is thrown, the assertion error exception is created with the
  parameter expression2(if applicable).
  An Example: assert list != null && list.size() > 0 : "list variable is null or empty";
  Object value = list.get(0);
