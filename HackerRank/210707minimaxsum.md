# Mini Max Sum

- <https://www.hackerrank.com/challenges/mini-max-sum/problem>

## Purpose

- prints the minimum and maximum combination of four integers

## My Solution

```java
public static void miniMaxSum(List<Integer> arr) {
        ArrayList<Long> finalsums = new ArrayList<Long>();
        for (int a = 0; a < arr.size(); a++){
            long sum = 0;
            for(int b = 0; b < arr.size(); b++){
                sum = sum + arr.get(b);
            }
            sum = sum - arr.get(a);
            finalsums.add(sum);
        }
        System.out.println(Collections.min(finalsums)+ " "+ Collections.max(finalsums));
    }
```