# Plus Minus

- <https://www.hackerrank.com/challenges/plus-minus/problem>

## My Solution

- returns proportion of positives, negatives, and zeroes

## Solution

```java
public static void plusMinus(List<Integer> arr) {
    // Write your code here
    float positive = 0;
    float negative = 0;
    float zero = 0;
    for (int a = 0; a < arr.size(); a++){
        if (arr.get(a) == 0){
            zero = zero+1;
            //System.out.println("z");
        }
        if (arr.get(a) < 0){
            negative = negative+1;
            //System.out.println("n");
        }
        if (arr.get(a) > 0){
            positive = positive+1;
            //System.out.println("p");
        }
        //System.out.println(arr.get(a));
        //System.out.println(positive+"\n" +negative+ "\n" + zero);
    }
    //System.out.println(arr.size());
    float p =positive/arr.size();
    float n = negative/arr.size();
    float z = zero/arr.size();
    System.out.println(p + "\n" + n+"\n" + z);

    }

```