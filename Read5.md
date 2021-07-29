# Linked List

Declare: Is a part of the collection framework present in `java.util` 

    Statment in Java
    LinkedList<String> linkedList  = new LinkedList<String>();

**Get an Example:**

    
    import java.util.*;
    public class Test {
        public static void main(String args[])
        {
            LinkedList<String> ll = new LinkedList<String>();
            ll.add("A");
            ll.add("B");
            ll.addLast("C");
            ll.addFirst("D");
            ll.add(2, "E");
            System.out.println(ll);
            ll.remove("B");
            ll.remove(3);
            ll.removeFirst();
            ll.removeLast();
    
            System.out.println(ll);
        }
    }
    /*OutPut: 
    [D, A, E, B, C]
    [A]*/

>In the last example you are shown how i can used the remove and add item to the linked list.

## When To Use
* It is best to use an ArrayList when:

    * You want to access random items frequently
    * You only need to add or remove elements at the end of the list

* It is best to use a LinkedList when:

    * You only use the list by looping through it instead of accessing random items
    * You frequently need to add and remove items from the beginning, middle or end of the list

**Other Method : `getFirst(ll);` used to return the first value of linked list**

>The starting point of the list is a reference to the first node, which is referred to as the head. Nearly all linked lists must have a head, because this is effectively the only entry point to the list and all of its elements, and without it, you wouldn’t know where to start! The end of the list isn’t a node, but rather a node that points to null, or an empty value.