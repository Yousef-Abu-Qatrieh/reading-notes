# Read: 03 - primitives, File I/O   
Java has two-fold type system:   

1-	Primitive data type like (int, byte,short,long,double,float,char,boolean)      
2-	Reference type like(Integer,Byte,Boolean,Double,Float,Character,Short,Long)      

Every primitive has reference type contains object we call it Wrapper class    
Java performs a conversion between the primitive and reference types if an actual type is different from the declared one:   
Integer j = 1; // autoboxing    
int i = new Integer(1); // unboxing  

The process of converting a primitive type to a reference one is called autoboxing, the opposite process is called unboxing.     
the primitive types are much faster and require much less memory. Therefore, we might want to prefer using them.       
The reference types are objects, they live on the heap and are relatively slow to access. They have a certain overhead concerning their primitive counterparts.    
# Exception
An exception is an event that occurs during the execution of a program that disrupts the normal flow of instructions.    
We use try and catch to handle the expected error     
There is 3 types of exceptions:          
1-	the checked exception. These are exceptional conditions that a well-written application should anticipate and recover from.    
2-	the error. These are exceptional conditions that are external to the application, and that the application usually cannot anticipate or recover from.    
3-	the runtime exception. These are exceptional conditions that are internal to the application, and that the application usually cannot anticipate or recover from   
 The throw statement requires a single argument: a throwable object. Throwable objects are instances of any subclass of the Throwable class   
#Scanner
We use scanner to read values form the user which can parse primitive types and strings using regular expressions.    
The resulting tokens may then be converted into values of different types using the various next methods.    
We use .close() to close the scanner   
Sorce: [Java Oracle](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/index.html)   
