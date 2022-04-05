## Linked List

A linked list can be seen as one of the little toy snakes you had as a kid. The ones with the joints that you could move around (see Ex. 2.1). The way I depict this is in Ex. 2.2. With Ex. 2.2, we see the head, the tail, and the components of the snake. With counting the head as 0, we can tell that the size of our snake is 4, and the capacity of our snake is 5. Size is how many spaces we have in our snake or linked list, whereas capacity is how many numbers we can hold in the snake.
###### Ex. 2.1
![image](https://user-images.githubusercontent.com/61299344/161401701-3c85f447-34f3-4cd9-8fdc-ed1234d017d6.png)

###### Ex. 2.2
![image](https://user-images.githubusercontent.com/61299344/161600615-3d3b5cf2-02c9-4400-a722-b1e473bd80d3.png)

Each element in a linked list is called a node. Each node has a pointer to the next node in the list, as well as a pointer to the previous node in the list. The Head is the first node in the list, whereas the tail is the last node. This is why I think of linked nodes as the toy snakes, so they are easier to visualize.

When we insert into a linked list, we need to consider whether we are inserting a new node at the head, the tail, or in the middle. With each scenario, there are different steps.

When inserting at the head, we have 4 basic steps:
> 1. We create a new node (usually calling it new_node).
> 2. Set the "next" of the new node to the current head (new_node.next = self. head)
> 3. Set the "previous" of the current head to the new node (self.head.prev = new_node)
> 4. Set the head equal to the new node (self.head = new_node)
When inserting at the head or the tail when the linked list is empty, we just need to set the head and the tail to the new node we have created.

Inserting at the tail is basically the same as inserting at the head. Instead of using self.head, we will just use self.tail, and we will set the "previous" of the new node to the tail first, then the "next: of the tail to the new node.

What this looks like:
> 1. Create a new node (new_node)
> 2. Set the "previous of the new node to the current tail (new_node.prev = self.tail)
> 3. Set the "next" of the current tail to the new node (self.tail.next = new_node)
> 4. Set the tail equal to the new node (self.tail = new_node)

Inserting a Node into the middle of a linked list is the most tedious out of the three.

Removing from a linked list is easier than inserting into a linked list.
If there is only one node in the list, then all that needs to be done is to set self.head and self.tail to None. This creates an empty linked list.

-	Basic features (insert, remove, access)
-	Finishing touches (remove, size, empty)
-	Example
-	Problem to Solve
