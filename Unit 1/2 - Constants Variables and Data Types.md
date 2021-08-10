# Constants Variables and Data Types

## Learning Objectives
- Be able to declare a constant
- Be able to declate a variable
- Know the difference between a constant and variable
- Name 4 different Data Types
- Describe what type inference is

## Constants

To store values in programming we use constants and variable. A constant is a value that is not going to change. If we were writing an app to represent a person the value of their name would be a constant. To create a constant we use the "let" keyword. Here is an example:

```Swift
	let name = "Alan"
```

## Variables

A variable is a value that could change in the future. If we take our previous example of a person the value of their age is going to change. To create a variable we use the "var" keyworked. Here is an example:

```Swift
	var age = 28
```
Perhaps their birthday is coming up if we want to change their age we can. We call the instance of the variable and set a new value. Here is an example:

```Swift
	age = 29
```

## Naming Conventions

When giving names to our constants and variables we use something called camelCase. The naming convention goes as following:
- No spaces
- First word is lower case
- Each word after has the first letter capitilized

It is helpful to be exact when naming our constants and variables. This makes it easier to recall and find variables and constants we have created. Here are some examples:

```Swift
	let nameOfFather = "Bob"
	var ageOfFather = 45
```

## Data Types

There are many types of Data Types in the Swift Language. We will cover a few of the basics here in this lesson.

### Strings
A string is a way to represent text. To create a string we use the quotes "". Everything inside of the quotes in considered part of the string. Here is an example:

```Swift
	let name = "Alan is really cool"
```

### Numbers
To represent numbers there are many different data types that are used. Here we will focus on two. **Int** and **Double**. Int stands for integer it is used to represent whole numbers. Doubles are used to represent numbers that have decimals. We will cover both ints and doubles more in the next lesson. Here are some examples of both:

```Swift
	let integer = 5
	let double = 5.1
```

### Booleans
Booleans are a way to represent whether a value is true or false. A Bool only has those two values, you can not set it to anything else. In our example of a person they could have a Bool to represent their married status. Here is an example:

```Swift
	let isMarried = true
```

In future lessons we will discuss how we can create our own custom data types.

## Type Inference
In all of the examples given in this lesson the swift compiler determines what type the value is. Swift is smart and can tell that 5 is an integer, or that "Alan is really cool" is a String. However there will be times that you want to be specific in what type you are declaring. You can do that in the definition of the variable. Here is how:
```Swift
	let name: String = "Alan"
```
Here we tell the compiler that name will most defintely be a String. This is not required to do, but can be helpful when you are first starting to get familiar with different data types.
