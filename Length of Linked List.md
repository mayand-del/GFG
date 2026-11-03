## 01. Length of Linked List

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/count-nodes-of-linked-list/1)

### Problem Description

**Task:** Given a singly linked list. Find the length of the linked list, where length is defined as the number of nodes in the linked list.Examples :Input: head: 1 - > 2 - > 3 - > 4 - > 5Output: 5

#### Examples

##### Example 1

- **Explanation:** Length of the linked list is 5, as there are 5 nodes present in it.

##### Example 2

- **Input:**
```text
head: 2 - > 4 - > 6 - > 7 - > 5 - > 1 - > 0 Output: 7
```
- **Explanation:** Length of the linked list is 7, as there are 7 nodes present in it.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-10-31 00:02:39
- **Status:** Correct
- **Marks:** 1

```cpp
/* Structure of linked list Node
class Node {
  public:
    int data;
    Node *next;

    Node(int x) {
        data = x;
        next = nullptr;
    }
};
*/
class Solution {
  public:
    int getCount(Node* head) {
        // Code here
        Node* temp=head;
        int count=0;
        while(temp!=NULL){
            temp=temp->next;
            count++;
        }
        return count;
    }
};
```

*Generated on: 03/11/2026, 22:05:04*