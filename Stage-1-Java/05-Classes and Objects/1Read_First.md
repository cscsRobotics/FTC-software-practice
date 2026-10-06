# Classes & Objects

So far, you have learned how to use variables, conditionals, loops, and methods. Now you are going to learn one of the most important parts of Java: **classes and objects**.

Classes allow you to organize related data and behavior together. You will use classes constantly when working with Java and FTC.

## What is a Class?

A **class** is like a blueprint. It describes what something has and what it can do.

For example, a robot might have:

- A name
- Motor power
- A claw state

And it might be able to:

- Drive
- Turn
- Open its claw
- Close its claw

A class can describe all of these things.

```java
class Robot {
    String name;
    double motorPower;

    void drive() {
        System.out.println("The robot is driving");
    }
}
```

Here, `Robot` is the class.

The variables inside the class are called **fields**. The method inside the class is a **method belonging to the class**.

## What is an Object?

An **object** is a specific instance of a class.

If `Robot` is the blueprint, an actual robot created from that blueprint is an object.

You can create an object using `new`:

```java
Robot myRobot = new Robot();
```

Now `myRobot` is an object created from the `Robot` class.

You can access its fields and methods using `.`:

```java
myRobot.name = "BioBuzz";
myRobot.motorPower = 0.5;

myRobot.drive();
```

The `.` is used to access something that belongs to the object.

## Class vs. Object

Think of it like this:

**Class:** describes what a robot is.

**Object:** an actual robot created using that description.

You can create multiple objects from the same class:

```java
Robot robot1 = new Robot();
Robot robot2 = new Robot();
```

Both objects are `Robot` objects, but they can have different values.

```java
robot1.name = "BioBuzz";
robot2.name = "PracticeBot";
```

## Why Does This Matter in FTC?

You have already been working with objects without necessarily thinking about them this way.

For example:

```java
DcMotor leftMotor;
```

`DcMotor` is a class/type, and `leftMotor` is a variable that can refer to a `DcMotor` object.

You can then use methods belonging to that object:

```java
leftMotor.setPower(0.5);
```

Understanding classes and objects will make it much easier to understand how FTC's Java libraries are organized.

## Before Moving On

Make sure you understand:

- What a class is
- What an object is
- What a field is
- What a method is
- What `new` does
- How to access an object's fields and methods using `.`
