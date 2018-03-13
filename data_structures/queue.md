## Data Structures

### Queue
Queue is an abstract data structure, somewhat similar to Stacks. Unlike stacks, a queue is open at both its ends. 
One end is always used to insert data (enqueue) and the other is used to remove data (dequeue). Queue follows 
First-In-First-Out methodology, i.e., the data item stored first will be accessed first.

[![Queue](https://www.tutorialspoint.com/data_structures_algorithms/images/queue_diagram.jpg)](https://www.tutorialspoint.com/data_structures_algorithms/dsa_queue.htm)

[Using List as a Queue](https://docs.python.org/3/tutorial/datastructures.html#using-lists-as-queues)

It is also possible to use a list as a queue, where the first element added is the first element retrieved 
(“first-in, first-out”); however, lists are not efficient for this purpose. While appends and pops from the end of list 
are fast, doing inserts or pops from the beginning of a list is slow (because all of the other elements have to be 
shifted by one).

To implement a queue, use collections.deque which was designed to have fast appends and pops from both ends.
```python
from collections import deque
queue = deque(["Eric", "John", "Michael"])
queue.append("Terry")           # Terry arrives
queue.append("Graham")          # Graham arrives
queue.popleft()                 # The first to arrive now leaves
'Eric'
queue.popleft()                 # The second to arrive now leaves
'John'
queue                           # Remaining queue in order of arrival
deque(['Michael', 'Terry', 'Graham'])
```
