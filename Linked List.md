## Linked List

A linked list can be seen as one of the little toy snakes you had as a kid. The ones with the joints that you could move around (see Ex. 2.1). The way I depict this is in Ex. 2.2. With Ex. 2.2, we see the head, the tail, and the components of the snake. With counting the head as 0, we can tell that the size of our snake is 4, and the capacity of our snake is 5. Size is how many spaces we have in our snake or linked list, whereas capacity is how many numbers we can hold in the snake.
###### Ex. 2.1
![image](https://user-images.githubusercontent.com/61299344/161401701-3c85f447-34f3-4cd9-8fdc-ed1234d017d6.png)

###### Ex. 2.2
![image](https://user-images.githubusercontent.com/61299344/161600615-3d3b5cf2-02c9-4400-a722-b1e473bd80d3.png)

Each element in a linked list is called a node. Each node has a pointer to the next node in the list, as well as a pointer to the previous node in the list. The Head is the first node in the list, whereas the tail is the last node. This is why I think of linked nodes as the toy snakes, so they are easier to visualize.

##### Inserting
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
> 2. Set the "previous" of the new node to the current tail (new_node.prev = self.tail)
> 3. Set the "next" of the current tail to the new node (self.tail.next = new_node)
> 4. Set the tail equal to the new node (self.tail = new_node)

Inserting a Node into the middle of a linked list is the most tedious out of the three. The process involves five steps instead of four, and what we need to do is connect all of the pieces so that our theoretical snake can move the way it's supposed to. If we don't connect all of those joints, then it will be broken. For our example, we are going to use "current" to reference the node before where we want to insert our new node. This would be O(n) in Big O Notation, which means the bigger the linked list, the longer inserting the node would take.

When inserting a new node into a linked list, it should go a little something like this:
> 1. Create a new node (new_node)
> 2. Set the "previous" of the new node to the current node (new_node.prev = current)
> 3. Set the "next" of the new node to the new next node (new_node.next = current.next)
> 4. Set the "previous" of the "next" node after "current" to the new node (current.next.prev = new_node)
> 5. Set the "next" of "current" to the new node (current.next = new_node)

#### Removing
Removing from a linked list is easier than inserting into a linked list. What needs to be done is removing a piece of this snake, and connecting the theoretical rope to the other pieces.

When removing the head, it's quite simple. You set the "next" to none, and you set the head to the second node.

This looks as such:
> self.head.next.prev = None
> self.head = self.head.next

When you remove the tail, it's similar to removing the head. You set the "previous" of the last node to none, and you set the tail to be the second to last node.

This looks like this:
> self.tail.prev.next = None
> self.tail = self.tail.prev

If there is only one node in the list, then all that needs to be done is to set self.head and self.tail to None. This creates an empty linked list.

When removing from the middle, it is definitely easier than inserting a None into the middle of a Linked List. For this example, we are going to use "current" for the node we are taking out of the list. This would be O(n) in Big O Notation, which means the bigger the linked list, the longer removing the node would take.

Steps to take:
> 1. Setting the "previous" of the Node after "current" to the Node before "current" (current.next.prev = current.prev)
> 2. Setting the "next" of the Node before "current to the Node after "current" (current.prev.next = current.next)

#### Accessing
When we want to find a value or finding a specific node, we have to loop through the linked list. To do this, we need to either start at the head or the tail. When we loop through the head, we need to follow the "next" until we reach the tail. When starting at the tail, we need to follow the "previous" until we reach the head.

#### Big O Notation
> inserting the head = O(1)

> inserting the tail = O(1)

> inserting in the middle = O(n)

> removing the head = O(1)

> removing the tail = O(1)

> removing in the middle = O(n)

> size = O(1)

> empty = O(1)

-	Example
-	Problem to Solve
