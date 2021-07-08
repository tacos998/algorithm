# Birthday Cake Candles

- <https://www.hackerrank.com/challenges/time-conversion/problem>

## Purpose

- converts time from a 12 hour clock system to a 24 hour clock system

## My Solution

```java
 public static String timeConversion(String s) {  
    int hours = Integer.parseInt(s.substring(0,2));
    String min = s.substring(3,5);
    String sec = s.substring(6,8);
    String ampm = s.substring(8,10);
    System.out.println(ampm);

    if (ampm.equals("AM") && hours > 0 && hours < 12){
        return s.substring(0,8);
    }
    if (hours == 12 && ampm.equals("PM")){
        return s.substring(0,8);
    }
    if (hours == 12 && ampm.equals("AM")){
        return "00:"+min+":"+sec;
    }
    else{
        return hours+12+":"+min+":"+sec;
    }

}
```