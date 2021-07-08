# Birthday Cake Candles

- <https://www.hackerrank.com/challenges/birthday-cake-candles/problem>

## Purpose

- returns the number of tallest birthday cake candles

## My Solution

```java
public static int birthdayCakeCandles(List<Integer> candles) {
    int maxNum = Collections.max(candles);
    int num = 0;
    for (int a = 0; a < candles.size(); a++){
        if (candles.get(a) == maxNum){
            num++;
        }
    }
    return num;

    }
```