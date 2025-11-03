# 🧮 Java Grade Calculator

A simple Java console program that calculates the average of student marks and displays the corresponding grade.

---

### 📘 Code Example
```java
public class GradeCalculator {
    public static void main(String[] args) {
        int[] marks = {90, 85, 80, 95, 88};
        int total = 0;

        for (int mark : marks) {
            total += mark;
        }

        double average = total / (double) marks.length;
        System.out.println("Average: " + average);

        if (average >= 90) System.out.println("Grade: A");
        else if (average >= 80) System.out.println("Grade: B");
        else if (average >= 70) System.out.println("Grade: C");
        else if (average >= 60) System.out.println("Grade: D");
        else System.out.println("Grade: F");
    }
}
