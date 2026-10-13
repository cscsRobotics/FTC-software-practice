### Practice 2: Methods and Object State

```java
class Robot {
    String name;
    double power;

    void setPower(double newPower) {
        power = newPower;
    }

    void boost(double amount) {
        power = power + amount;
    }

    void showStatus() {
        System.out.println(name + " has power " + power);
    }
}

Robot robot1 = new Robot();
Robot robot2 = new Robot();

robot1.name = "Alpha";
robot2.name = "Beta";

robot1.setPower(0.5);
robot2.setPower(0.7);

robot1.boost(0.2);
robot2.boost(0.1);

robot1.showStatus();
robot2.showStatus();
```

**Questions**

1. What is `robot1.power` after `robot1.setPower(0.5)`?
2. What is `robot1.power` after `robot1.boost(0.2)`?
3. What is `robot2.power` after both of its method calls?
4. What gets printed by each `showStatus()` call?
5. Explain how `setPower()` changes the object's `power` field.
6. If `robot1.boost(0.5)` is called, does it affect `robot2.power`? Why?
7. What is the difference between the parameter `amount` and the field `power`?
