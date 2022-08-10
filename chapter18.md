# Chapter 18: Memory Management

Removing, adding, and inserting items to a long arraylist can be taxing on memory

Solution? use storage that does not require contiguous bits of memory

Linked List! Each item contains data and a reference to the next item in the list
Items can be stored anywhere in memory
Quick insert and removal, but access can take longer because the list must be traversed in order; uses more memory due to storing a link

List node consists of data to be stored, and reference to next node in list

**Int Node**
public class IntNode {
   private int dataVal;         // Node data
   private IntNode nextNodePtr; // Reference to the next node

   public IntNode() {
      dataVal = 0;
      nextNodePtr = null;
   }

   // Constructor
   public IntNode(int dataInit) {
      this.dataVal = dataInit;
      this.nextNodePtr = null;
   }

   // Constructor
   public IntNode(int dataInit, IntNode nextLoc) {
      this.dataVal = dataInit;
      this.nextNodePtr = nextLoc;
   }

   /* Insert node after this node.
    Before: this -- next
    After:  this -- node -- next
    */
   public void insertAfter(IntNode nodeLoc) {
      IntNode tmpNext;

      tmpNext = this.nextNodePtr;
      this.nextNodePtr = nodeLoc;
      nodeLoc.nextNodePtr = tmpNext;
   }

   // Get location pointed by nextNodePtr
   public IntNode getNext() {
      return this.nextNodePtr;
   }

   public void printNodeData() {
      System.out.println(this.dataVal);
   }
}

## Heap/Stack

Code: program instructions stored here
Static memory: static fields live here- addresses do not change
Stack: method's local variables live here; calling a method adds variables to the stack, return removes them (automatic memory)
Heap: where "new" operator allocates memory for objects (free store)

## Garbage collection

Program finds unused, unreachable memory locations and frees memory

Java keeps a *reference count* of reference variables currently referring to an object
Reference count = 0 = unreachable object
Memory deallocation of unreachable objects occurs next time Java VM invokes the garbage collector

Local reference variables declared within a method automatically have their reference count decremented upon method return