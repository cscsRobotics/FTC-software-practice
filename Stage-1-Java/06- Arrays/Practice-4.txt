# Practice 4: Debugging Arrays

Each code snippet contains a problem. Identify and fix it.

### Problem 1

```java
int[] scores = {70, 80, 90};

System.out.println(scores[3]);
```

1. What is wrong with this code?
2. Rewrite the statement so it prints the last element.

### Problem 2

```java
int[] numbers = {1, 2, 3, 4};

for (int i = 0; i <= numbers.length; i++) {
    System.out.println(numbers[i]);
}
```

1. Why does this loop fail?
2. Fix the loop condition.

### Problem 3

```java
double[] motorPowers = {0.3, 0.5, 0.7};

motorPowers[3] = 1.0;
```

1. Why is the assignment invalid?
2. Rewrite it to change the last element to `1.0`.

### Problem 4

```java
String[] motorNames = {"FrontLeft", "FrontRight", "BackLeft"};

System.out.println(motorNames.length());
```

1. What is the problem?
2. Rewrite the statement correctly.
