## Welcome!
Hello! My name is Jane Orr, and I am a Software Engineering student at BYU-Idaho. This is a basic introduction to a few Data Structures that are commonly used in the industry. The Data Structures we are going to go over are Stacks, Linked Lists, and Trees. You may be confused on what these are now, but I assure you: it will become a lot clearer after you read this tutorial of sorts.
Contact Information:
Jane Orr
Orr19002@byui.edu

## Stack
A stack can easily be represented by a stack of something we all know and love: pancakes. 
  In a stack of pancakes, you start eating the last pancake that was put on the stack. A stack can be referenced as a LIFO Data Structure, which stands for 
  “Last In, First Out”. The top of the stack can be referred to as the back of the stack, whereas the bottom can be referred to as the front of the stack. 
  This can be confusing, but what needs to be remembered is the front of the stack is in reference to the first item in the stack, or as in our example, 
  the first pancake on the plate. 

###### Ex: 1.1
 ((NOTE TO SELF: ADD PICTURE HERE)

When we add a value, or a pancake, to our stack, it is added to the top. This is called a push operation. This pushes everything down to make room for 
  the new value, and we can add that value to the back of the stack. When we remove a value, or eat a pancake off the top, or the back, of the stack, 
  that is called the pop operation. When we use the push and pop operations, it is always off the back of the stack (the top of the stack).
Now, when you eat a stack of pancakes, you don’t eat it starting with the bottom pancake. You don’t eat it starting from the middle. 
  You start from the top and work your way down. This is where the LIFO part comes in. When you interact with a stack, 
  it needs to be from the top down. This makes it a good data structure to remember where we have been, but not so much a good 
  data structure with data being consistently rotated.

###### Ex: 1.2
Push: 
5								    6
3		<-		+6		=		    5
1								    3
								    1

Pop:
6								    5
5		<-		-6		=		    3
3								    1
1								

Along with push and pop, there are a couple of other operations that can be used with stacks. These are called size() and empty(). 
  These do exactly as they say: figure out the size of the stack, or empty the contents of the stack. 
  
All operations that are performed in a stack are O(1) operations. This means that in Big O Notation, no matter how big or small the
  stack may be, all operations will take the same amount of time. This is very important in the world of coding, as it is the most
  efficient type of Big O Notation.
  
-	Example
-	Problem to Solve

## Linked List

A linked list can be seen as one of the little toy snakes you had as a kid. The ones with the 
-	Introduction
-	Visual Representation (Snake)
-	Basic features (insert, remove, access)
-	Finishing touches (remove, size, empty)
-	Example
-	Problem to Solve

## Tree
-	Introduction
-	Visual Representation
-	Basic Features (rules, balance)
-	BST Operations (insert, traversing)
-	Finishing touches (contains, height, size, empty)
-	Example
-	Problem to Solve