# Vector analysis

## Why should there be vector?
When we code to solve problem, we alway use array to store and deal with data. But we alway don't know how big the array should be. If it is too small, the program don't work, well, if it is too large, it should waste a lot of memory. In order to fix the problem, vector appear. 

Vector is sequence container representing array that can change in size. User do not need to consider the size of Array.

## How vector work?
The basic idea of vector is that when we use out of space, we alloc a new big space and remove datas to new space, then free the old space. 

We suppose the size of old space is n, and how much should the size of new space be? Obviously n+1 is not a good idea because if we add one more element to the vector, it should alloc new space and remove data again. how about n+2,n+3...? A clever strategy is 2*n which is used be by many implementations of STL.


## What can we learn from the implementation of vector?

