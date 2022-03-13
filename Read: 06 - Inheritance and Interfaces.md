# Read: 06 - Inheritance and Interfaces
## Object   
An object is a software bundle of related state and behavior. Software objects are often used to model the real-world objects that you find in everyday life. This explains how state and behavior are represented within an object.   

## Class
A class is a blueprint or prototype from which objects are created. This defines a class that models the state and behavior of a real-world object. It intentionally focuses on the basics, showing how even a simple class can cleanly model state and behavior.    

## Inheritance
Different kinds of objects often have a certain amount in common with each other.   
Object-oriented programming allows classes to inherit commonly used state and behavior from other classes.   
each class is allowed to have one direct superclass, and each superclass has the potential for an unlimited number of subclasses.   
The syntax for creating a subclass is simple. At the beginning of your class declaration, use the extends keyword, followed by the name of the class to inherit from.    

## Interfaces
In the Java programming language, an interface is a reference type, similar to a class, that can contain only constants, method signatures, default methods, static methods, and nested types. Method bodies exist only for default methods and static methods.    
Interfaces cannot be instantiated—they can only be implemented by classes or extended by other interfaces.   
Defining an interface is similar to creating a new class:

public interface OperateCar {

   // constant declarations, if any

   // method signatures
 
   int changeLanes(Direction direction,   
                   double startSpeed,   
                   double endSpeed);   
   int signalTurn(Direction direction,   
                  boolean signalOn);   
   int getRadarFront(double distanceToCar,   
                     double speedOfCar);   
   int getRadarRear(double distanceToCar,   
                    double speedOfCar);   
         ......  
}  
Note that the method signatures have no braces and are terminated with a semicolon.   
To use an interface, you write a class that implements the interface. When an instantiable class implements an interface, it provides a method body for each of the methods declared in the interface.   

Source:[OracleWebsite](https://docs.oracle.com/javase/tutorial/java/)
