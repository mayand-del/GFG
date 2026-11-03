## 01. Linked List Traversal

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-linked-list-elements/1)

### Problem Description

**Task:** Given the head of a singly linked list, return an array containing the values of its nodes.Examples:Input: Output: [1, 2, 3, 4, 5]

#### Examples

##### Example 1

- **Explanation:** The linked list contains 6 elements [10, 20, 30, 40, 50, 60]. The elements are printed in a single line.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-10-31 00:06:19
- **Status:** Correct
- **Marks:** 1

```cpp
/*
class Node {
  public:
    int data;
    Node* next;

    // Default constructor
    Node() {
        data = 0;
        next = NULL;
    }

    // Parameterised Constructor
    Node(int data) {
        this->data = data;
        this->next = NULL;
    }
};
*/
class Solution {
  public:
    vector<int> printList(Node *head) {
        // code here
        vector<int>ans;
        
        Node* temp=head;
        
        while(temp!=NULL){
            ans.push_back(temp->data);
            temp=temp->next;
        }
        return ans;
    }
};
```

*Generated on: 03/11/2026, 22:02:02*