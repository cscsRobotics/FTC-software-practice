### Practice 3: Predict the Output

Do not run the code. Trace the changes to each object.

```java
class Robot {
    String name;
    int battery;

    void useBattery(int amount) {
        battery = battery - amount;
    }

    void recharge(int amount) {
        battery = battery + amount;
    }

    void showBattery() {
        System.out.println(name + ": " + battery);
    }
}

Robot robot1 = new Robot();
Robot robot2 = new Robot();

robot1.name = "Alpha";
robot1.battery = 100;

robot2.name = "Beta";
robot2.battery = 80;

robot1.useBattery(25);
robot2.useBattery(10);
robot1.recharge(5);

robot1.showBattery();
robot2.showBattery();
```

**Questions**

1. What is `robot1.battery` after `useBattery(25)`?
2. What is `robot2.battery` after `useBattery(10)`?
3. What is `robot1.battery` after `recharge(5)`?
4. What is the complete output?
5. Why does recharging `robot1` not change `robot2.battery`?
6. Which fields belong to each object?
