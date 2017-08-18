# Important topics on Java.

* ### [Inheritance](https://github.com/pkvarnwal/JavaAndCollection/edit/master/README.md#Inheritance)

* ### Polymorphism
* ### Interface
* ### Abstract
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



