# Migratory Birds

- <https://www.hackerrank.com/challenges/migratory-birds/problem>

## Purpose

- returns the type with the highest frequency. If the frequency is the same, returns the lowest type

## My Solution

```java
public static int migratoryBirds(List<Integer> arr) {
    HashMap<Integer, Integer> frequency = new HashMap<Integer,Integer>();
    for (int a = 0; a < arr.size(); a++){
        int temp = arr.get(a);
        if (frequency.containsKey(temp)){
            frequency.replace(temp, frequency.get(temp)+1);
        }
        else {
            frequency.put(temp, 1);
        }
    }
    int current = arr.get(0);
    for (int b : frequency.keySet()){
        if (frequency.get(current) < frequency.get(b)){
            current = b;
        }
        if (frequency.get(current) == frequency.get(b)){
            current = Math.min(current, b);
        }
    }
    return current;
    }
```