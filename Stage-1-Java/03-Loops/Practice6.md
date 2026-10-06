Practice 6 - FTC

Consider:
```java
while (opModeIsActive()) {

    if (gamepad1.a) {
        claw.setPosition(1.0);
    }

    if (gamepad1.b) {
        claw.setPosition(0.0);
    }

}
```
Answer:

1. Why is the while loop useful here?
2. What is the program repeatedly checking?
3. What happens when A is pressed?
4. What happens when B is pressed?
5. Why would this be better than checking the buttons only once?
