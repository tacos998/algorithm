# Grading Students

- <https://www.hackerrank.com/challenges/grading/problem>

## Purpose

- rounds student grades according to guidelines

## My Solution

```java
public static List<Integer> gradingStudents(List<Integer> grades) {
    for (int a = 0; a < grades.size(); a++){
        int temp = grades.get(a);
        if (temp >=38){
            if (temp%5 == 3){
                grades.set(a, temp+2);
            }
            if (temp%5 == 4){
                grades.set(a, temp+1);
            }  
    }
    }
    return grades;
    }
```