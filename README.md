# AP Computer Science A - 2D Array Lab

## Overview
In this lab, you must utilize a two-dimensional array. There may be other ways to manage this task, but you are required to use a two-dimensional array. The approach you take to solving these problems is up to you, but you must follow the method specifications below.

## Main Driver Method
Set up a two-dimensional array where each row corresponds to a student, and each column corresponds to a class. Each entry is the GPA that the student has in each class.

### Example:
```
          Class 0  Class 1  Class 2
Student 0   3.2      2.8      3.1
Student 1   4.0      3.8      3.9
Student 2   3.6      3.9      3.1
Student 3   2.5      2.6      2.1
Student 4   3.8      4.0      3.5
```

## Basic Lab Requirements
1. **Display the 2D Array**
   ```java
   /**
    * Displays the 2D array of grades in a readable format with headers and labels.
    * @param gradeChart The 2D array representing students' GPAs.
    * @precondition gradeChart is not null.
    * @postcondition The array is printed to the console.
    */
   public static void displayGradeChart(double[][] gradeChart)
   ```

2. **Calculate Class Average**
   ```java
   /**
    * Computes and returns the average GPA for a specified class.
    * @param gradeChart The 2D array representing students' GPAs.
    * @param col The column index representing the class.
    * @return The average GPA for the class.
    * @precondition col is a valid index within gradeChart.
    * @postcondition No changes to gradeChart.
    */
   public static double classAVG(double[][] gradeChart, int col)
   ```

3. **Calculate Student Average**
   ```java
   /**
    * Computes and returns the average GPA for a specified student.
    * @param gradeChart The 2D array representing students' GPAs.
    * @param row The row index representing the student.
    * @return The average GPA for the student.
    * @precondition row is a valid index within gradeChart.
    * @postcondition No changes to gradeChart.
    */
   public static double studentAVG(double[][] gradeChart, int row)
   ```

4. **Search for a Specific GPA**
   ```java
   /**
    * Searches for a specific GPA in the 2D array.
    * @param gradeChart The 2D array representing students' GPAs.
    * @param gpa The GPA to search for.
    * @return true if the GPA is found, false otherwise.
    * @precondition gradeChart is not null.
    * @postcondition No changes to gradeChart.
    */
   public static boolean findGPA(double[][] gradeChart, double gpa)
   ```

5. **Find the Best GPA in a Class**
   ```java
   /**
    * Finds the student with the highest GPA in a specified class.
    * @param gradeChart The 2D array representing students' GPAs.
    * @param col The column index representing the class.
    * @return The row index of a student with the highest GPA in that class.
    * @precondition col is a valid index within gradeChart.
    * @postcondition No changes to gradeChart.
    */
   public static int bestGPA(double[][] gradeChart, int col)
   ```


## Lab Extensions
These extensions are optional but will enhance your program. Document which ones you complete in your file header.

1. **Handle Ties for Best GPA in a Class**
   ```java
   /**
    * Finds all students with the highest GPA in a specified class.
    * @param gradeChart The 2D array representing students' GPAs.
    * @param col The column index representing the class.
    * @return An ArrayList of student row indices with the highest GPA.
    * @precondition col is a valid index within gradeChart.
    * @postcondition No changes to gradeChart.
    */
   public static ArrayList<Integer> bestGPAsWithTies(double[][] gradeChart, int col)
   ```

2. **Find the Student with the Highest Overall GPA**
   ```java
   /**
    * Finds and displays the student(s) with the highest overall GPA.
    * @param gradeChart The 2D array representing students' GPAs.
    * @param studentNames The array of student names corresponding to rows.
    * @precondition gradeChart and studentNames are not null and have matching dimensions.
    * @postcondition The name(s) and GPA(s) of the highest student(s) are displayed.
    */
   public static void bestStudent(double[][] gradeChart, String[] studentNames)
   ```
