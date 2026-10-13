### Practice 4: One Class, Multiple Objects

```java
class Motor {
    String location;
    double power;

    void setPower(double newPower) {
        power = newPower;
    }

    void stop() {
        power = 0.0;
    }
}

Motor leftMotor = new Motor();
Motor rightMotor = new Motor();

leftMotor.location = "Left";
rightMotor.location = "Right";

leftMotor.setPower(0.6);
rightMotor.setPower(0.8);

rightMotor.stop();
```

**Questions**

1. How many objects were created?
2. What is `leftMotor.power` at the end?
3. What is `rightMotor.power` at the end?
4. Does calling `rightMotor.stop()` stop the left motor object? Explain.
5. Do both objects use the same class definition?
6. If you added a `reverse()` method to the `Motor` class, could both objects call it?
7. Explain the difference between the `Motor` class and the `leftMotor` object.
