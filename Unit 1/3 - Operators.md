# Operators

## Learning Objectives

- How to do basic mathematics operations
- How to add two numbers of different types together
- How to find the remainder of a division operation

## Assign A value

To assign a value the = operator is used. The left side of the = is what is being set. The right side of the = is the value. Here is an example:
```Swift
	let number = 5
```
Here we are setting the constant of number. The value we are setting it to is 5. The = operator can often be confused with the == operator. The == operator will be covered more in the next lesson, but it is a way to check if two values are the same.

## Basic Mathematics Operators

Adding, subtracting, multiplying, and dividing are all built into the Swift language. All of the operators that are familiar are the same (+, -, \*, /) Here is an example of how each would be used
```Swift
	let addition = 5 + 2
	let subtraction = 5 - 2
	let multiplication = 5 * 2
	let dividing = 4 / 2
```
The values of the code snippet above would be as follows:
- Addition - 7
- Subtraction - 3
- Multiplication - 10
- Dividing - 2

*Best Practice* - It is best to put spaces between your basic mathematics operators. This makes your code more easily readable and familiar to others.


## Remainder Operator

When dividing the numbers will not always come out as whole numbers. Dividing 5 / 2 is 2 remainder 1. In swift you can get the remainder by using the % operator. Here is an example:
```Swift
	let dividing = 5 / 2 // This results in 2 
	let remainder = 5 % 2 // This results in 1
```
In this example dividing is the result of 2 because we are diving Int or whole numbers. The remainder is 1, because that is how many left over after a full division.

## Type Conversion
Numbers have two types that will be used to start. The first is *Int* which means it's a whole number. The second is *Double* which means it has the potential to be more than a whole number. If using mathematics operators the numbers have to be the same type. Here are some examples:
```Swift
	let x = 10 // Int
	let y = 5.2  // Double
```
In order to do math with x and y they must be converted to match. Below is two examples of how you could do that:
```Swift
	let doubleResult = Double(x) + y
	let intResult = x + Int(y)
```
The value of the code snippet above would be as follows:
- doubleResults- 15.2
- intResult - 15
When converting a Double to an Int it will round to the nearest whole number. This is just the beginning of type conversion. In future lessons we will do more complex type conversions.
