# Stage 1: Java Basics
# Lesson 6: Arrays

## Goal

By the end of this lesson, you should understand:

- What an array is and why it is useful.
- How to declare and initialize an array.
- How to access and change array elements.
- How array indexes work.
- How to use `.length`.
- How to loop through an array.
- How arrays can be useful in robotics programming.

---

## 1. What Is an Array?

An **array** is a variable that stores multiple values of the same type.

Imagine you want to store the power values of four motors.

Without an array, you might write:

```java
double frontLeftPower = 0.5;
double frontRightPower = 0.5;
double backLeftPower = 0.5;
double backRightPower = 0.5;
```

That works, but it becomes inconvenient when you have many values to manage.

With an array, you can store them together:

```java
double[] motorPowers = {0.5, 0.5, 0.5, 0.5};
```

Now, all four values are stored in one array called `motorPowers`.

An array has a fixed length, meaning its number of elements cannot change after it is created.

## 2. Declaring and Initializing Arrays

The general syntax is:

```java
dataType[] arrayName = {value1, value2, value3};
```

Examples:

```java
int[] scores = {90, 85, 100};
double[] powers = {0.2, 0.5, 0.8};
String[] motorNames = {"FrontLeft", "FrontRight", "BackLeft"};
boolean[] motorWorking = {true, true, false};
```

The type before the brackets determines what kind of values the array stores.

- `int[]` stores integers.
- `double[]` stores decimal numbers.
- `String[]` stores strings.
- `boolean[]` stores boolean values.

All elements in an array must be compatible with its declared type.

You can also create an array with a specific length:

```java
int[] scores = new int[5];
```

This creates an array with five integer elements. Each element initially contains `0`.

For an array of `double`, the default value is `0.0`. For `boolean`, it is `false`. For reference types such as `String`, it is initially `null`.

## 3. Array Indexes

Each element in an array has an **index**, which identifies its position.

Java array indexes start at `0`, not `1`.

For example:

```java
int[] scores = {90, 85, 100, 75};
```

| Index | Value |
|---:|---:|
| 0 | 90 |
| 1 | 85 |
| 2 | 100 |
| 3 | 75 |

The first element is at index `0`, and the last element is at index `3`.

To access an element, write the array name followed by the index in square brackets:

```java
System.out.println(scores[0]); // Prints 90
System.out.println(scores[2]); // Prints 100
```

Remember: the index is the position, not the value stored there.

## 4. Changing Array Elements

You can change an individual element by assigning a new value to its index.

```java
int[] scores = {90, 85, 100};

scores[1] = 95;

System.out.println(scores[1]); // Prints 95
```

The array is now:

```java
{90, 95, 100}
```

Only the element at index `1` changed. The other elements remain the same.

## 5. The `.length` Property

Every array has a `length` property that tells you how many elements it contains.

```java
int[] scores = {90, 85, 100, 75};

System.out.println(scores.length); // Prints 4
```

Notice that `.length` is a property, not a method. You write `scores.length`, not `scores.length()`.

Since array indexes start at `0`, the last valid index is:

```java
scores.length - 1
```

For an array of four elements, the valid indexes are `0` through `3`.

Trying to access an index outside the array's valid range causes an `ArrayIndexOutOfBoundsException`.

For example:

```java
int[] scores = {90, 85, 100};

System.out.println(scores[3]); // Error at runtime
```

There are only three elements, so the valid indexes are `0`, `1`, and `2`.

## 6. Looping Through Arrays

Arrays become especially useful when combined with loops.

Suppose you want to print every score:

```java
int[] scores = {90, 85, 100, 75};

for (int i = 0; i < scores.length; i++) {
    System.out.println(scores[i]);
}
```

Here's how the loop works:

1. `int i = 0` starts the index at `0`.
2. `i < scores.length` keeps the loop running while the index is valid.
3. `i++` increases the index by one after each iteration.
4. `scores[i]` accesses the element at the current index.

The loop prints each value in order.

### Enhanced for loop

Java also has an enhanced `for` loop, which is useful when you want to process every element without needing its index.

```java
int[] scores = {90, 85, 100, 75};

for (int score : scores) {
    System.out.println(score);
}
```

The variable `score` holds the current element during each iteration.

Use a traditional `for` loop when you need the index or need to modify elements by position. Use an enhanced `for` loop when you simply want to process each element.

## 7. Arrays in Robotics

Arrays can help organize related data in an FTC program.

For example, you might keep track of four motor power values:

```java
double[] motorPowers = {0.5, 0.5, 0.5, 0.5};

for (int i = 0; i < motorPowers.length; i++) {
    System.out.println("Motor " + i + ": " + motorPowers[i]);
}
```

This prints the power value associated with each index.

You could also store target encoder positions, sensor readings, or a series of recorded values.

**Important:** this example only stores and prints numbers. It does not control actual FTC motors. Real hardware requires motor objects and appropriate SDK calls.

---

## Before Moving On

Make sure you can:

- [ ] Explain what an array is.
- [ ] Declare and initialize arrays of different types.
- [ ] Access an element using its index.
- [ ] Change an element's value.
- [ ] Explain why the first index is `0`.
- [ ] Use `.length` to determine the number of elements.
- [ ] Loop through an array using a traditional `for` loop.
- [ ] Explain the difference between a traditional `for` loop and an enhanced `for` loop.

If you can do these without copying the examples, you're ready for the practice problems.
