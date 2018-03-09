## Data Structures

### Linked List
A linked list is a sequence of data structures, which are connected together via links.

A linked List is a sequence of links which contains items. Each link contains a connection to another link. 
A linked list is the second most-used data structure after array. Following are the important terms to understand 
the concept of Linked List.

[![Linked List](https://www.tutorialspoint.com/data_structures_algorithms/images/linked_list.jpg)](https://www.tutorialspoint.com/data_structures_algorithms/linked_list_algorithms.htm)

```python
class Node :
	def __init__( self, data ) :
		self.data = data
		self.next = None
		self.prev = None

class LinkedList :
	def __init__( self ) :
		self.head = None		

	def add( self, data ) :
		node = Node( data )
		if self.head == None :	
			self.head = node
		else :
			node.next = self.head
			node.next.prev = node						
			self.head = node			

	def search( self, k ) :
		p = self.head
		if p != None :
			while p.next != None :
				if ( p.data == k ) :
					return p				
				p = p.next
			if ( p.data == k ) :
				return p
		return None

	def remove( self, p ) :
		tmp = p.prev
		p.prev.next = p.next
		p.prev = tmp		

	def __str__( self ) :
		s = ""
		p = self.head
		if p != None :		
			while p.next != None :
				s += p.data
				p = p.next
			s += p.data
		return s

# example code
l = LinkedList()

l.add( 'a' )
l.add( 'b' )
l.add( 'c' )

print l
l.remove( l.search( 'b' ) )
print
print l

```
