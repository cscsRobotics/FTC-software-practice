# Stage 1: Java
## 04 - Methods

### Goal

Learn how to create reusable blocks of code and call them when needed.

---

## 1. What is a method?

A method is a named block of code that performs a specific task.

Instead of writing the same code multiple times, you can put it inside a method and call the method whenever you need it.

Example:

```java
void sayHello() {
    System.out.println("Hello!");
}
```
The method does not run just because it was created.

You have to call it:
```java

sayHello();

```
## 2. Method Structure

A basic method looks like this:
```java
returnType methodName() {
    // code
}
```
Example:
```java
void driveForward() {
    System.out.println("Driving forward");
}
Parts of the method
void driveForward() {
    System.out.println("Driving forward");
}
```
void = the method does not return a value
driveForward = the method's name
() = parameters go here
{ } = contains the code that runs when the method is called

## 3. Calling a `=method

Creating a method:
```java
void driveForward() {
    System.out.println("Driving forward");
}
```
Calling the method:
```java
driveForward();
```
You can call it multiple times:
```java
driveForward();
driveForward();
driveForward();
```
The code inside the method runs each time it is called.

## 4. Parameters

A method can receive information through parameters.

Example:
```java
void setPower(double power) {
    System.out.println(power);
}
```
You can call it with:
```java
setPower(0.5);
```
Here:
```java
power = 0.5
```
You can also call:
```java
setPower(1.0);
```
Now:
```java
power = 1.0
```
The value passed into the method is called an argument.

The variable inside the method's parentheses is called a parameter.

A method with no parameters runs a fixed block of code without needing any input values.

An integer literal would look like this:

```java
void print5() {
System.out.println(5); 

}

print5();
```
here are no parameters, so the method requires no arguments when it is called. 

And if you call the method, it will always print the number 5.

## 5. Multiple parameters

A method can have more than one parameter.
```java
void drive(double leftPower, double rightPower) {
    System.out.println(leftPower);
    System.out.println(rightPower);
}
```
Call it with:
```java
drive(0.5, 0.5);
```
Now:
```java
leftPower = 0.5
rightPower = 0.5
```
## 6. Returning a value

A method does not always have to be void.

It can return a value.

Example:
```java
int add(int a, int b) {
    return a + b;
}
```
You can store the returned value:
```java
int result = add(3, 4);
```
Now:
```java
result = 7
```
The return statement sends the result back to wherever the method was called.

## 7. Methods in FTC

Methods are useful for organizing robot actions.

For example:
```java
void openClaw() {
    claw.setPosition(1.0);
}
```
Then instead of repeatedly writing:
```java
claw.setPosition(1.0);
```
you can simply write:
```java
openClaw();
```
Another example:
```java
void setDrivePower(double left, double right) {
    leftMotor.setPower(left);
    rightMotor.setPower(right);
}
```
Then:

setDrivePower(0.5, 0.5);

This sets both motors to 0.5.
