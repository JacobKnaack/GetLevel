# Get Level

Code Challenge: Find the level of a given value in a Binary Tree.

> Write a program that can find the tree level of a value stored in Binary Tree.

## Example Inputs and Outputs

### Case 1: Shallow Search

Input:

```text
BT  ---->   1           value  ---->  3
          /   \    
        2      3
      /                  
    4                    
```

Output: 1

### Case 2: Deep Search

Input:

```text
BT  ---->   1           value  ---->  9
          /   \    
        2      3
      /   \   /  \         
     4     5 6    7
    / \
   8   9
```

Output: 3

### Case 3: Null Search

Input:

```text
BT  ---->   1           value  ---->  8
          /   \    
        2      3
      /   \   /  \         
    4      5 6    7
```

Output: null

## Algorithm

* Initialize a counter for level starting at 0
* Check if a node exists -> if not return null
* Check if node value equals the search value
  * If value exists return counter for level
  * If value does not exist increment level
    * Check left side using incremented level
    * Check right side using incremented level
