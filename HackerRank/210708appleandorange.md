# Apple and Orange

- <https://www.hackerrank.com/challenges/apple-and-orange/problem>

## Purpose

- returns the number of apples and oranges that fall in the house

## My Solution

```java
public static void countApplesAndOranges(int s, int t, int a, int b, List<Integer> apples, List<Integer> oranges) {
    List<Integer> applesf = new ArrayList<Integer>();
    List<Integer> orangesf = new ArrayList<Integer>();
    int houseapples = 0;
    int houseoranges = 0;
    for (int i = 0; i < apples.size(); i++){
        applesf.add(apples.get(i)+a);
    }
    for (int j = 0; j < oranges.size(); j++){
        orangesf.add(oranges.get(j)+b);
    }
    for (int k = 0; k < applesf.size(); k++){
        if (applesf.get(k) >= s && applesf.get(k) <=t){
            houseapples++;
        }
    }
    for (int l = 0; l < orangesf.size(); l++){
        if (orangesf.get(l) >= s && orangesf.get(l) <=t){
            houseoranges++;
        }
    }
    System.out.println(houseapples+ "\n"+houseoranges);
    }
```