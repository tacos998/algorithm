# Kangaroo

- <https://www.hackerrank.com/challenges/kangaroo/problem>

## Purpose

- returns whether the two kangaroos will meet at a certain point

## My Solution

```java
public static String kangaroo(int x1, int v1, int x2, int v2) {
    if ((x1 < x2 && v1 > v2) || (x1 > x2 && v1 < v2)){
        if ((x1 - x2) % (v2 - v1) == 0){
            return "YES";
        }
        else{
            return "NO";
        }
    }
    else{
        return "NO";
    
    
    }
```