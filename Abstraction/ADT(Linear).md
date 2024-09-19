# Abstract Data Type (ADT)
ADTs are the mental model for how data will be organized and accessed.
9/10 the content of ADTs are data structures - objects that organize other objects like a list, array, or arraylist.

# Stack: a simple linear ADT
A fundamental abstraction and its mental model can be a stack of books.
Similar in Java, the most recent method call is at the top and appropriately should finish first (add and remove from the top without problem)
Vertical data structure that does not branch (linear) only interact at the top.

public interface StackADT<E> {
    public void push (E element);

    public E pop ();

    ...
}

Again, these methods in the interface need documentation (the overall mental model)