# Functions

## Learning Objectives
- How to write a function
- Know what a parameter and return type are
- Be able to use a tuple
- How to use default parameters

## Why Use Functions
A function is used when you want to re-use a chunk of code instead of writing it over and over again. An example would be calculating score. Maybe in your app you calculate the score on many screens. Instead of writing that same piece of code for every screen you can do it just once. Then you can call that function every place you need it. Anytime you are copying and pasting code in your project there is a good chance it would be better served in a function.

## How to declare a function

To declare a function you start with the keyword "func". Then, you name your function (Remember it's always better to be expressive). After the name comes parenthesis. To finish you put a return type and two curly braces. Here is an example:
```Swift
	func thisIsTheNameOfMyFunction() {
		// Write code here for your function
	}
```

## Parameters and Return Types

*Parameters* are a way to pass information into the function. Perhaps the function needs two numbers that it can add together. You can use parameters to give the function those numbers. Parameters can be of any Data Type. The parameters go inside the parenthesis. First you name the parameter then the colon followed by the data type. Commas between each parameter and you can have as many as you want. Here is an example:

```Swift
	func nameOfFunction(parameterOne: String, parameterTwo: Double) {
		print(parameterOne) // Gives the value that was passed into the function
		print(parameterTwo) // Gives the value that was passed into the function
	}
	nameOfFunction(typeOne: "Hello", typeTwo: 20)
```

*Return Type* is a way to give back information to whatever is calling the function. In the case of an addition function you would want to know what the result of the function was. To add a return type after the parenthesis use "->" then the data type you need to return. Inside the function you then need to return the result. Of note no code after a return will be executed, so make sure that returning is the last thing that happens in the function. Here are some examples:

```Swift
	func nameOfFunction() -> String {
		return ""
	}
	let result = nameOfFunction()
	// result is now the value of whatever is returned from the function
```

Putting it all together example:
```Swift
	func add(numberOne: Double, numberTwo: Double) -> Double {
		let result = numberOne + numberTwo
		return result
	}
	let addition = add(numberOne: 5, numberTwo: 3)
	print(addition) // 8
```

### Default parameters

With parameters you can also set a default value. Perhaps the value will be the same most of the time. By adding a default parameter that value won't be required when calling the function. You add a default parameter by adding a "=" after the data type then the value. Here is an example:

```Swift
	func adding(numberOne: Double = 5, numberTwo: Double) -> Double {
    	let result = numberOne + numberTwo
    	return result
	}
	adding(numberTwo: 5)
```

## Tuples
Lastly, tuples are a way that you can return multiple values. In the case of functions there will be times that returning two or more values is helpful. Tuples are made by two parenthesis and the data types that you want to use. Here is an example:
```Swift
	func adding(numberOne: Double = 5, numberTwo: Double) -> (Double, String) // Returns a tuple {
    	let result = numberOne + numberTwo
    	return (result, "you did it!") // Returns two values in a tuple
	}
```


