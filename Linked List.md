## Linked List

A linked list can be seen as one of the little toy snakes you had as a kid. The ones with the joints that you could move around (see Ex. 2.1). The way I depict this is in Ex. 2.2. With Ex. 2.2, we see the head, the tail, and the components of the snake. With counting the head as 0, we can tell that the size of our snake is 4, and the capacity of our snake is 5. Size is how many spaces we have in our snake or linked list, whereas capacity is how many numbers we can hold in the snake.
###### Ex. 2.1
![image](https://user-images.githubusercontent.com/61299344/161401701-3c85f447-34f3-4cd9-8fdc-ed1234d017d6.png)

###### Ex. 2.2
![image](https://user-images.githubusercontent.com/61299344/161600615-3d3b5cf2-02c9-4400-a722-b1e473bd80d3.png)
Each element in a linked list is called a node. Each node has a pointer to the next node in the list, as well as a pointer to the previous node in the list. The Head is the first node in the list, whereas the tail is the last node. This is why I think of linked nodes as the toy snakes, so they are easier to visualize.

When we insert into a linked list, we need to consider whether we are inserting a new node at the head, the tail, or in the middle. With each scenario, there are different steps.
When inserting at the head, we have 4 basic steps:


-	Basic features (insert, remove, access)
-	Finishing touches (remove, size, empty)
-	Example
-	Problem to Solve
