# Linked_List_loop_detection_and_removal
Sometime in singly Linked list , the last node of LL starts pointing to one of the node , creating Loops in Linked list. This code will detect loop in Linked list and remove that loop.

Pseudo Code-

1. Detecting loop
    1.1 Traverse Linked list using 2 pointer one slow and second fast pointer.
    1.2 In one go , Slow pointer will jump to next node and fast pointer will jump to next to next node.
    1.3 If these 2 pointers meet at same node---- It means Linked List contain loop.
    1.4 If these 2 pointer do not meet then ----- It means Linked List contain NO Loops
 2. Using Floyd's cycle - Finding alogorithm , we will find the starting node of loop.
 3. Remove loop 
  3.1 call detect loop function and store the meeting node of fast and slow pointer in a pointer called meet_node.
  3.2 Move head pointer and meet_node one by one and return the last node of the loop.
  3.3 make the next pointer last node of loop to Null. Hence loop removed
