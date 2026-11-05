## 01. Swap Odd and Even Bits

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/swap-all-odd-and-even-bits-1587115621/1)

### Problem Description

**Task:** Given an unsigned integer n, You have to swap all even-position bits with their rightside adjacent odd-position bits.

#### Examples

##### Example 1

- **Input:**
```text
n = 23Output: 43Explanation: Binary representation of the given number is 00010111 after swapping 00101011 = 43 in decimal.
```

##### Example 2

- **Input:**
```text
n = 2
```
- **Output:**
```text
1
```
- **Explanation:** Binary representation of the given number is 10 after swapping 01 = 1 in decimal.

#### Constraints

- **1.** `1 ≤ n ≤ 10⁹`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-05 22:21:04
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public int swapBits(int n) {
        // code here
        int even=n & 0xAAAAAAAA;
        int odd=n& 0x55555555;
        even= even>>1;
        odd=odd<<1;
        
        return even | odd;
    }
}
```

*Generated on: 05/11/2026, 22:22:01*