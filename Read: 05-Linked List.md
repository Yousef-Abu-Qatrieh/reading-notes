# Big (O) notation  
we use big o notation to measure:   
1- time complexity   
2- space complexity   

time complexity : The amount of time a function needs to complete.   
space complexity : The amount of memory resources a function uses to store data and instructions.   
## Role of Big O 
big o algorithm efficiency is to describe the Worst Case of efficiency an algorithm can have in performing it’s job   
#### Factor for anlayise Big o  
1-Input Size   
2-Units of Measurement   
3-Orders of Growth   
4-Best Case, Worst Case, and Average Case   

Input Size refers to the size of the parameter values that are read by the algorithm    
To evaluate a function for Time and Space complexity    

We can describe overall efficiency by using the input size n and measuring the overall Units of Space and Time required for the given input size n  

![image](https://user-images.githubusercontent.com/97651232/157287626-06a8f7f3-9e3a-48d0-b3eb-605959bb886c.png)   


Big O: The worst case analysis of algorithm efficiency.    
Running Time: The amount of time required for an algorithm to complete.     
Memory Space: The amount of memory resources required for an algorithm to complete.    
Input Size: Represented by the variable n, the total size of values used as parameters in an algorithm.      
Big Omega: The best case analysis of algorithm efficiency.       
Big Theta: The typical or random case used for analysis of algorithm efficiency.     

![image](https://user-images.githubusercontent.com/97651232/157287925-6235b7ce-442d-436b-84c6-13b07dddee25.png)   

# Linked Lists
A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.   
Terminology:   
Linked List - A data structure that contains nodes that links/points to the next node in the list.   
Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.   
Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.   
Node - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.   
Next - Each node contains a property called Next. This property contains the reference to the next node.   
Head - The Head is a reference of type Node to the first node in a linked list.   
Current - The Current is a reference of type Node to the node that is currently being looked at. When traversing, you create a new Current variable at the Head to guarantee you are starting from the beginning of the linked list.   
Source: [Codefellows](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)
