Java source file if I compile
Java compiler generate .class file. This .class file I have to give as input to JVM. Then JVM is responsible to load and execute .class file.
Now this .class input to class loader subsystem.

## Class Loader SubSystem:

There are three types of Class Loader:

## Loading: In the loading there are multiple parts:
## Linking:
## Initialization:

## Loading:

* Bootstrap class loader
* Extension class loader: It is child of BootStrap
* Application class loader: It is child of Extension

It is called Delegation Heirerchy Alorythm:

## Linking:

* Verify
* Prepare
* Resolve

## Initialization:

* Initialization

First of all Loading will be executed then Linking will be executed and then Initialization will be executed.

So, Class Loader SubSystem is the responsible for the Loading, Linking, Initialization.


Whatever .class file input to Class Loader Subsystem, this Class Loader System is responsible to load our classes.
While loading to load, some memory must be required. For executing some memory must be required. 

## What are various memory area present inside JVM: 

## Memory Area of JVM:

* Method Area: Class data will be there. Static method will be stored
* HEAP Memory Area: Object data and corresponding instance variable will be there, Array is also stored in Heap Area
* STACK Area: For every Thread a seperate Run Time Stack will be created:
Ex: T1, T2, ....Tn
Eack entry in Stack is called Stack Frame. Every Stack Frame contain, three part of there: 
* Local variable Array
* Frame Data
* Operand Stack

So, for every thread a seperate Stack will be there, all local variable will be stored in the corresponding Run time Stack.


* PC Register: PC Register for T1, PC Register for T2, PC Register for Tn

For every thread a saperate PC Register will be created, for every thraed a saperate Runtime Stack will be created. But for total JVM one HEAP Area, 
One Method Area by default will be there.


* Native Method Stack: For every Thread a separate Stack by default will be there.
Ex: T1, T2, ...Tn



.class file came which is produced by Java Compiler, .class file access input to Class Loader SubSystem.
Class Loader SubSystem dumped our .class file in the Method Area. Now who is responsible to execute our program: Execution Engine.

## Execution Engine:

Execution Engine contain mainly two parts are:
1. Interpreter
2. JIT Compiler

## JIT Compiler: 
* Intermediate Code Generator: produces Intermediate code
* Code Optimizer: is responsible to optimize that code.

