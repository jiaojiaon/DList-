# DList-The actual linked lists built into C++ work almost exactly like the doubly linked lists described
in class, except that they use a very cool heuristic. Instead of maintaining head and tail
references such that head.previous = null and tail.next = null, they maintain a reference to one
special node called “the sentinel node” or “nil.”
This node replaces the null references so that a NullPointerException can never be thrown. The
sentinel node has the following properties:
 sentinel.previous = what we used to call the tail
 sentinel.next = what we used to call the head
 what we used to call the tail . next = sentinel
 what we used to call the head . previous = sentinel
In effect this node replaces null, and maintaining a reference to it replaces having to maintain
separate head and tail references. 
