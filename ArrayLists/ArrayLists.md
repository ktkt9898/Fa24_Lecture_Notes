# Interface "ADT" Implementation Separation
Recall a list interface defines the operations and expected behavior of a list, but does not specify how a list implementation will manage list elements internally.

# What if list elements are stored in an array?
Advantages:
Linear organization, easy to visualize
Big O(1) constant, very fast lookup by index

Disadvantages:
Arrays do not automatically move, grow, or shrink elements and costs Big O(n) time operations.

