# Breaking the Records

- <https://www.hackerrank.com/challenges/breaking-best-and-worst-records/problem>

## Purpose

- returns the number of times the record score max and min were broken

## My Solution

```java
public static List<Integer> breakingRecords(List<Integer> scores) {
    int max = scores.get(0);
    int maxC = 0;
    int min = scores.get(0);
    int minC = 0;
    for (int a = 0; a < scores.size(); a++){
        if (scores.get(a)>max){
            max = scores.get(a);
            maxC++;
        }
        if (scores.get(a)<min){
            min = scores.get(a);
            minC++;
        }
    }
    ArrayList<Integer> result = new ArrayList<Integer>();
    result.add(maxC);
    result.add(minC);
    
    return result;
    }
    }
```