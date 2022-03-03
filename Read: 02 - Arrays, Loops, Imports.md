# Read: 02 - Arrays, Loops, Imports

## Array

Array is data structure that allow you to store sequence of value that are all from the same type    
In java array are objects    
In java we can store primitive in array or we can store object reference type   
all data in array must be in the same type    
### Create array  
There is 3 ways to create array      
1-	Primitive data type [] name Of Array; array declaration no memory space.     
             Ex: double [] salaries;
2-	Primitive data type [] name Of Array = {value, value, value, value, value}; declaration and initialization only work if we know the size of array and the data that we want to add.    
Ex: int [] marks = {1,2,3,4,5};

3-	Primitive data type [] name Of Array = new Primitive data type [size of array]; declaration and memory allocated if we know the size of array and we don’t know the data that we want to initialize it.     

Ex: String [] names = new String [5];     
#### To add element to the array that we declare:    
           Name of array [index] = value;
           Ex: names [0] =” Jordan”;
The index of array is starting from zero    
If we try to add data to array for index not exist it will give this error index out of bounds
 We can create multi-dimensional array
Ex: int [] [] matrix = new int [rows][columns];
To add element for 2 dimensional array
Ex: matrix[0][0] =23;
## Packages 
Is organize group of classes together   
The statement order is as follows.
1.	Package statement (optional).
2.	Imports (optional).
3.	Class or interface definitions.
Ex: package example;   
       import java.util.*   
       public class Main {}      
##### Common Imports
There are 166 packages containing 3279 classes and interfaces in Java 5. However, only a few packages are used in most programming. GUI programs typically use at least the first three imports.    
import java.awt.*;	Common GUI elements.    
import java.awt.event.*;	The most common GUI event listeners.    
import javax.swing.*;	More common GUI elements. Note "javax".    
import java.util.*;	Data structures (Collections), time, Scanner, etc classes.    
import java.io.*;	Input-output classes.    
import java.text.*;	Some formatting classes.   
import java.util.regex.*;	Regular expression classes.    

## Loops   
we use loop to execute code certain number of times    
There is 3 types of loops   
1- for loop  is a control structure that allows us to repeat certain operations by incrementing and evaluating a loop counter.   
ex  for(intial ;condition;increment){}
2- while loop The while loop is Java's most fundamental loop statement. It repeats a statement or a block of statements while its controlling Boolean-expression is true.   
ex while (condition){ we can do increment inside it};    
3- do while loop it will execute our code at least one    
ex do{statements}while(condition);    


Sorce: [Java Oracle](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/index.html) 
