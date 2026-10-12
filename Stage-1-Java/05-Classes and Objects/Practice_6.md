### Practice 6: Build Your Own

Create a class called `Robot` with these fields:

- `String name`
- `int battery`
- `double power`

Add these methods:

- `useBattery(int amount)`: subtracts the given amount from `battery`.
- `recharge(int amount)`: adds the given amount to `battery`.
- `setPower(double newPower)`: changes the robot's power.
- `showStatus()`: prints the robot's name, battery, and power.

Then:

1. Create two different `Robot` objects.
2. Give each object a different name, battery level, and power.
3. Call `useBattery()` on the first object.
4. Call `recharge()` on the second object.
5. Change the power of the first object.
6. Print both objects' statuses.
7. Explain why the two objects can have different field values even though they come from the same class.
