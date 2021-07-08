# Staircase

- <https://www.hackerrank.com/challenges/staircase/problem>

## My Solution

- returns a staircase of size n

## Solution

```java
public static void staircase(int n) {
        for (int a = 0; a < n; a++){
            for (int b = 0; b < n-a-1; b++){
                System.out.print(" ");
            }
            for (int c = 0; c <= a; c++){
                System.out.print("#");
            }
            System.out.print("\n");
        }
        
    }
```