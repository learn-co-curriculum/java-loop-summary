# Summary of Loops

## Learning Goals

- Show one problem and how we can implement it with any of the loops we learned
  about.
- Discuss when certain loops should be used.

## Introduction

Consider the problem statement:

Assume we want to print the integers from 0 to 5. So we'd expect the program
to print numbers 0, 1, 2, 3, 4, 5.

We can use any of the loops we have learned to accomplish this task. Consider
the following program:

```java
public class LoopExample {
  public static void main(String[] args) {
      
    // Implement a for loop that prints the integers 0 - 5
    System.out.println("The For Loop prints:");
    for (int i = 0; i <= 5; i++) {
      System.out.println(i);
    }

    // Implement a while loop that prints the integers 0 - 5
    System.out.println("\nThe While Loop prints:");
    int currentNumber = 0;
    while (currentNumber <= 5) {
      System.out.println(currentNumber);
      currentNumber++;
    }

    // Implement a do-while loop that prints the integers 0 - 5
    System.out.println("\nThe Do-While Loop prints:");
    currentNumber = 0;
    do {
      System.out.println(currentNumber);
      currentNumber++;
    } while (currentNumber <= 5);

  }
}
```

The output of this program would look like this:

```text
The For Loop prints:
0
1
2
3
4
5

The While Loop prints:
0
1
2
3
4
5

The Do-While Loop prints:
0
1
2
3
4
5
```

As we can see by the output, each loop accomplishes exactly what the problem
statement asks for; however, is there a loop that is more suited for this
problem?

In this lesson, we will learn about when to appropriately use each loop.

## What Loop to Use and When

Consider the following universal rules when using loops in programming:

- Use a `for` loop when it is known how many iterations of the loop should run.
- Use a `do-while` loop when it is known that the loop should iterate through at
  least once.
- Use a `while` loop when it is not known how many iterations of the loop should
  run.

To help with this, let's look at a flowchart:

![loop-flowchart](https://curriculum-content.s3.amazonaws.com/java-mod-1/loop-summary/what-loop-to-use-flowchart.png)

Using these rules and the flowchart here, we can determine which loop is best
suited for certain problem statements.

Now let's go back to the question we asked: Is there a loop that is more suited
for this problem?

The answer is a `for` loop. We know exactly how many times the loop should
re-iterate: 6 times. The other loops are best used in situations where we do not
know how many times we should iterate through.

Consider some examples of when to use each loop:

- Use a `for` loop when we know the loop should execute N number of times.
  - Like in our example above!
- Use a `for` loop when we want to iterate over an array.
  - We'll learn more about arrays soon!
- Use a `do-while` loop for menu-driven programs that depend on termination
  from the user.
  - See the "Do-While Loops" lesson for an example of a menu-driven program.
- Use a `while` loop when asking the user for input.
  - See the "While Loops" lesson for an example. Notice that the user could
    completely bypass the `while` loop by entering a certain input.
- Use a `while` loop for reading in a file.

## Conclusion

While we _can_ use either a `for` loop, a `while` loop, or a `do-while` loop
to accomplish a problem statement, it is worth reiterating when to use each
loop. The example described in the introduction is better suited for a `for`
loop rather than a `while` or `do-while` loop since we know exactly how many
times the loop should iterate over itself. When programming, consider the
following universal rules on when to use each loop:

- Use a `for` loop when it is known how many iterations of the loop should run.
- Use a `do-while` loop when the number of iterations known is at least once.
- Use a `while` loop when it is not known how many iterations of the loop should
  run.
