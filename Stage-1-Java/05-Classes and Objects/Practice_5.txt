### Practice 5: Find and Fix the Errors

A student wrote the following code:

```java
class Robot {
    String name;
    double power;

    void setPower(double newPower) {
        power = newPower;
    }

    void showStatus() {
        System.out.println(name + " has power " + power);
    }
}

Robot robot1 = new Robot();
Robot robot2 = new Robot();

robot1.name = "Alpha";
robot2.name = "Beta";

robot1.setPower(0.7);
robot2.setPower(0.3);

robot1.power = 0.9;

robot1.showStatus();
robot2.showStatus();
```

**Questions**

1. What does the code print as written?
2. Is there a programming error in the code? Explain.
3. Why does `robot1.power = 0.9` not change `robot2.power`?
4. Rewrite the final section so that both robots have their power set using `setPower()`, with Alpha at `0.2` and Beta at `0.6`.
5. What advantage might a method like `setPower()` have over directly changing a field?
