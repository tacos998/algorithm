# A Very Big Sum

- <https://www.hackerrank.com/challenges/a-very-big-sum/problem>

## Purpose

- returns sum of all numbers in the list

## My Solution

```java
public static long aVeryBigSum(List<Long> ar) {
        long sum = 0;
        for (int a = 0; a < ar.size(); a++){
            sum = sum + ar.get(a);
        }
        return sum;
    }
```