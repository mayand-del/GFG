## 01. Simple Interest

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/simple-interest3457/1)

### Problem Description

**Task:** Given three integers p, r and t, denoting Principal, Rate of Interest and Time period respectively. Calculate and print the Simple Interest.

#### Examples

##### Example 1

- **Input:**
```text
p = 100, r = 20, t = 2
```
- **Output:**
```text
40.00
```
- **Explanation:** The simple interest on 100 at a rate of 20% across 2 time periods is 40.

##### Example 2

- **Input:**
```text
p = 999, r = 9, t = 9
```
- **Output:**
```text
809.19
```
- **Explanation:** The simple interest on 999 at a rate of 9% across 9 time periods is 809.19

#### Constraints

- **1.** `1 ≤ p ≤ 10⁵¹ ≤ r, t ≤ 100`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-15 22:17:33
- **Status:** Correct
- **Marks:** 1

```java
import java.util.Scanner;
import java.math.BigDecimal;
import java.math.RoundingMode;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        BigDecimal P = sc.nextBigDecimal();
                BigDecimal R = sc.nextBigDecimal();
                BigDecimal T = sc.nextBigDecimal();

                // Formula: (P * R * T) / 100 aur 2 decimal places tak fix karna
                BigDecimal SI = P.multiply(R)
                                 .multiply(T)
                                 .divide(BigDecimal.valueOf(100), 2, RoundingMode.HALF_UP);

                // Answer print karna (e.g., 500.00)
                System.out.println(SI.toPlainString());
    }
}
```

*Generated on: 15/11/2026, 22:18:17*