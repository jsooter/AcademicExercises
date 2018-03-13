## Data Structures

### Stack
A stack is an Abstract Data Type (ADT), commonly used in most programming languages. It is named stack as it behaves 
like a real-world stack, for example – a deck of cards or a pile of plates, etc.

[![Stack](https://www.tutorialspoint.com/data_structures_algorithms/images/stack_representation.jpg)](https://www.tutorialspoint.com/data_structures_algorithms/stack_algorithm.htm)

[Using Lists as Stacks](https://docs.python.org/3/tutorial/datastructures.html#using-lists-as-stacks)

The list methods make it very easy to use a list as a stack, where the last element added is the first element retrieved (“last-in, first-out”). To add an item to the top of the stack, use append(). To retrieve an item from the top of the stack, use pop() without an explicit index.
```python
class stack(list):
    def push(self, item):
        self.append(item)
    def isEmpty(self):
        return not self
```
