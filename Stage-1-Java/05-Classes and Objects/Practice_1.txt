### Practice 1: Understanding Objects

Read the code and answer the questions.

```java
class Robot {
    String name;
    double power;

    void drive() {
        System.out.println(name + " is driving");
    }
}

Robot robot1 = new Robot();
Robot robot2 = new Robot();

robot1.name = "BioBuzz";
robot1.power = 0.8;

robot2.name = "PracticeBot";
robot2.power = 0.4;

robot1.drive();
robot2.drive();
```

**Questions**

1. How many objects are created?
2. What is the value of `robot1.name`?
3. What is the value of `robot2.power`?
4. What gets printed when `robot1.drive()` is called?
5. What gets printed when `robot2.drive()` is called?
6. If `robot1.name` changes to `"Alpha"`, does `robot2.name` change too? Explain why or why not.
7. Which part of the code defines the `Robot` class?
8. Which lines create the objects?
