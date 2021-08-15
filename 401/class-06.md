## What Does Singleton Mean?
A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object. This is helpful usually when a single object is required to coordinate actions across a system.

The singleton pattern is used in programming languages such as Java and .NET to define a global variable. A single object used across systems remains constant and needs to be defined only once rather than many times



## Techopedia Explains Singleton
A singleton is intended to provide only one instance of itself while facilitating a global point of access. Implementing a singleton pattern involves creating a class with a method that creates a new instance of the class. In order to implement a singleton pattern, principles of single instance and global access must be satisfied. The singleton class is like a global repository for an instance of itself, making the constructor private. Therefore, an instance outside the class cannot be created at all, and a singleton can contain only one instance. A singleton class instantiates itself and maintains that instance across systems.

Abstract factory, builder and prototype patterns can use singletons. Façade objects and static objects are often singletons. Singleton implementation requires a mechanism through which a class member can be accessed without having to create a class object and hold on to the value of class members among class objects. The steps involved in creating a singleton are as follows:


The constructor is made private. This allows only the class to have access to the singleton.

Example:

        class testdata
        {
        Private testdata ()
        {
//… no-op for a singleton

A single internal instance of the class is created using a method. The method is called an instance in this example. The method “instance” is used to initialize the class to access a single instance. The instance method is marked as static in this example to give all the threads consistent access. Outside the instance creation, the “lock” statement is used to control multithreaded access. This locks the instance creation to a single thread.

![](https://opensource.com/sites/default/files/uploads/designpatterns2_singletonpattern.jpg)


## Node.js Design Patterns — Singleton pattern ( Series -1)

### What are Design Patterns?

So what exactly are design patterns? Well, every day that we’re building software, we are usually presented with a lot of challenging problems, problems that we might have already solved. When presented with re-occurring problems, we are faced with a decision. Solve the problem again and again for each application where it occurs, or solve the problem once and for all with an improved solution, a pattern, a solution that you can use over and over again in any type of application where this problem occurs. If you find your solution works well by proving it in various applications and situations, and you feel like you can safely use your solution a million times over, it might be time to make it official.


Give your solution a name. Document your solution, evangelize it. Get other developers using your solution to solve the same problem when they face it. You will have just created a design pattern. Design patterns are reusable, reliable solutions to problems that we face every day in software development. Design patterns are named, cataloged solutions. They are well-tested and reusable in many different situations. They are well-documented so other developers can learn them, and they are easy to talk about with other engineers who already know them.
They make your code better and your applications less brittle. It’s easier to add new features or modules to applications where you use them. Although some design patterns may be difficult to learn at first, they ultimately simplify your code. Their aim is to present solutions for decoupling objects or modules and reducing the overall complexity of your architecture. Not only will understanding design patterns make you write better code, they will make you a better programmer, because learning design patterns gives you techniques that you can use when faced with common programming problems and a knowledge base that is easy to discuss at, say, an interview.
As a programmer who wants to write better code and reflect on better ways of doing things, learning and using design patterns is a must.
So in this series of node.js design pattern i am first going to put focus on Creation Design Pattern


## The Singleton Problem
Sometimes you need to make sure that you have one and only one instance of an object. This is where the singleton pattern can be useful. A singleton represents a single instance of an object. Only one can be created, no matter how many times the object is instantiated. If there’s already an instance, the singleton will create a new one. Let’s take a look at where creating multiple instances of one object might create problems within our application.
Lets create some files in node.js. First file is Logger.js.


        class Logger {

    constructor() {
        this.logs = [];
    }

    get count() {
        return this.logs.length;
    }

    log(message) {
        const timestamp = new Date().toISOString();
        this.logs.push({ message, timestamp });
        console.log(`${timestamp} - ${message}`);
    }

    }

    module.exports = Logger;