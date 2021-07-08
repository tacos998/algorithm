# Simple Array Sum

- https://www.hackerrank.com/challenges/simple-array-sum/problem
- Solved with a for loop

## Source Code

```java

public static int simpleArraySum(List<Integer> ar) {
    // Write your code here
    int sum = 0;
    for (int a = 0; a < ar.size(); a++){
        sum = sum + ar.get(a);
    }
    
    return sum;
    }

```
