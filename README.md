# Important topics on Java.

* ### [Inheritance](https://github.com/pkvarnwal/JavaAndCollection/blob/master/README.md#inheritance)

* ### [Polymorphism](https://github.com/pkvarnwal/JavaAndCollection/blob/master/README.md#polymorphism)
* ### [Interface](https://github.com/pkvarnwal/JavaAndCollection#interface-1)

* ### [Abstract](https://github.com/pkvarnwal/JavaAndCollection/blob/master/README.md#abstract)
* ### Interface Implementation
* ### Nested Interface
* ### Interface Variable
* ### Marker Interface
* ### Spannable Interface
* ### Interface vs Inheritance

* ### Inheritance: 
This is one way of achieving both polymorphism and code reuse at the same time.
Inhritance is when a `class` derives from an existing `class`.

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
