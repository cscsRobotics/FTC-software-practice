### DO NOT OPEN ANSWER KEY UNTIL YOU HAVE FINISHED ALL PRACTICE PROBLEMS!!! ###

# Practice 1

1. How many objects are created?
2. What is the value of `robot1.name`?
3. What is the value of `robot2.power`?
4. What gets printed when `robot1.drive()` is called?
5. What gets printed when `robot2.drive()` is called?
6. If `robot1.name` changes to `"Alpha"`, does `robot2.name` change too? Explain why or why not.
7. Which part of the code defines the `Robot` class?
8. Which lines create the objects?

-ANSWER-

1. There are two new objects created from the Robot class
2. The value of robot1.name is Biobuzz
3. The value of robot2.power is 0.4
4. When robot1.drive() is called, "BioBuzz is driving" is printed.
5. When robot2.drive() is called, "PracticeBot is driving" is printed.
6. If robot1.name changes to "Alpha" then robot2.name does not change. The objects have different instances; therefore, changing one field of one object does not affect the other object.
7. class Robot { ... }
8. ``` Robot robot1 = new Robot(); and Robot robot2 = new Robot ```


# Practice 2

1. What is `robot1.power` after `robot1.setPower(0.5)`?
2. What is `robot1.power` after `robot1.boost(0.2)`?
3. What is `robot2.power` after both of its method calls?
4. What gets printed by each `showStatus()` call?
5. Explain how `setPower()` changes the object's `power` field.
6. If `robot1.boost(0.5)` is called, does it affect `robot2.power`? Why?
7. What is the difference between the parameter `amount` and the field `power`?

-ANSWER-

1. 0.5
2. 0.7
3. 0.8
4. for robot1.showStatus(); "Alpha has power 0.7" gets printed. for robot2.showStatus(); "Beta has power 0.8" gets printed
5. power = newPower in the method for setPower, so when the parameter newPower has an argument of some number, it temporarily has that value whilst power retains that value until it is changed.
6. If robot1.boost(0.5) is called, it does not affect robot2.power because they are separate objects.
7. The parameter amount is a temporary value used by the method to apply the argument to the field power (so that power has a new value)


# Practice 3

1. What is `robot1.battery` after `useBattery(25)`?
2. What is `robot2.battery` after `useBattery(10)`?
3. What is `robot1.battery` after `recharge(5)`?
4. What is the complete output?
5. Why does recharging `robot1` not change `robot2.battery`?
6. Which fields belong to each object?

-ANSWER-

1. 75
2. 70
3. 80
4. robot1 complete output is "Alpha: 80" and robot2 complete output is "Beta: 70"
5. They are two separate objects; therefore, changes applied in one object will not affect the other.
6. all fields belong to each object because they are both instances made from the same Robot class. 


# Practice 4

1. How many objects were created?
2. What is `leftMotor.power` at the end?
3. What is `rightMotor.power` at the end?
4. Does calling `rightMotor.stop()` stop the left motor object? Explain.
5. Do both objects use the same class definition?
6. If you added a `reverse()` method to the `Motor` class, could both objects call it?
7. Explain the difference between the `Motor` class and the `leftMotor` object.

-ANSWER-

1. two objects were created from the Motor class. 
2. 0.6
3. 0.0
4. it does not stop the left motor object because the method stop() is only applied to the rightMotor object, not the left.
5. Yes, both motors use the same class definition.
6. Both objects could call a new 'reverse()' method because both objects use the same class definition. 
7. the leftMotor object is an instance of the Motor class


# Practice 5

1. What does the code print as written?
2. Is there a programming error in the code? Explain.
3. Why does `robot1.power = 0.9` not change `robot2.power`?
4. Rewrite the final section so that both robots have their power set using `setPower()`, with Alpha at `0.2` and Beta at `0.6`.
5. What advantage might a method like `setPower()` have over directly changing a field?

-ANSWER-

1. robot1.showStatus prints "Alpha has power 0.9" and robot2.showStatus prints "Beta has power 0.3"
2. There is not an error in the code; however, the field of power is directly changed instead of the method setPower being changed to 0.9
3. ;-; I think it's obvious enough. Every practice asks a question like this.
4. robot1.setPower(0.2); and robot2.setPower(0.6);
5. encapsulating power inside of setPower can put safe guards in place to prevent impossible or dangerous values from setting. 


# Practice 6

1. Create two different `Robot` objects.
2. Give each object a different name, battery level, and power.
3. Call `useBattery()` on the first object.
4. Call `recharge()` on the second object.
5. Change the power of the first object.
6. Print both objects' statuses.
7. Explain why the two objects can have different field values even though they come from the same class.

Well it's all up to you. The answer can vary. 
