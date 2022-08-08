# Chapter 18: Memory Management

Removing, adding, and inserting items to a long arraylist can be taxing on memory

Solution? use storage that does not require contiguous bits of memory

Linked List! Each item contains data and a reference to the next item in the list
Items can be stored anywhere in memory
Quick insert and removal, but access can take longer because the list must be traversed in order; uses more memory due to storing a link

