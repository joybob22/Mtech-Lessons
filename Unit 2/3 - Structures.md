# Structs

## Learning Objectives

- How to create a struct
- Be able to describe what value type means
- Be able to add functions to structs

## Declaring a struct

Structs are a way to create custom data types. Structs can be created for any purpose and are very commonly used. Structs are a great way to create a blueprint for the data needed in a project. to declare a struct you start with the "struct" keyword, then name the Struct, after open the curly braces. Inside the curly braces place all of the variables with the data types that will exist in the struct. Here is an example:

```Swift
	struct Person {
    	let name: String
    	let age: Int
	}
```

With this struct we have a blueprint and can create people using this person struct. To do this we need to use initializers.

## Initializers

Initializers are used to create instances of a struct. In structs initializers are given by default. You do not need to add an initializer for the struct to work. Using the Person struct above here is how you would create a person from the struct:

```Swift
	let kate = Person(name: "Kate", age: 26) // Created an instance of Person
	let cliff = Person(name: "Cliff", age: 68) // Created a different instance of Person
```
Here kate and cliff are instances of Person, meaning that they are variables created by using the default *memberwise* initializer given by the struct. Memberwise means that it's using the base default initializer provided by the struct.

Initializers can also be *custom*. That means you can set default values in the structs, or take in added information to help create an instance of a struct. Here is an example of a custom initializer.
```Swift
	struct Person {
    	let name: String
    	let age: Int
    	
    	init(firstName: String, lastName: String, age: Int) {
        	self.name = firstName + lastName
        	self.age = age
    	}	
	}
```
Here we use the custom initializer to get the first name and last name then combine them to set the value of the name on the Person. Note that we are using the "self" keyword here. Self refers back to the Parent class. In this case self.age is referring back to the name constant on the struct. Meanwhile age is referring to the parameter from the initializer function. 

## Value type

Structs are a value type. That means when you create a copy of a struct it creates a completely new copy. Here is an example:

```Swift
	struct Person {
    	let name: String
    	var age: Int
	}
	var kate = Person(name: "kate", age: 26)
	let anotherPerson = kate
	kate.age += 1
	print(kate.age) // prints 27
	print(anotherPerson.age) // prints 26
```

## Added functionality

Structs can do more than just be a blueprint of variable. They can also have functions to give added functionality to what the struct can do. There are two types of functions that can be created.

*Instance Methods* are helpful to give the struct access to the variables of the struct. Here is an example:
```Swift
	struct Size {
		var width: Double
		var height: Double

		func area() -> Double {
			width * height
		}
	}

```
*Mutating Methods* are used when there are changes made to the variable on a struct. To do this use the "mutating" keyword to show that the function is going to change variables of the struct. Here is an example:
```Swift
	struct Person {
    	let name: String
    	var age: Int
    
    	mutating func birthdayHappened() {
        	self.age += 1
    	}
	}
```

## Computed Properties
A helpful way to simplify computations is to make computed properties. That means there is logic done every time a variable is called. These are useful and can be used whenever desired. Here is an example of how to make one:
```Swift
	var nameOfMyVariable: Double {
		// Do the logic or compute value to return the value for the variable
	}
```
### Property Observers
Along with computed properties Swift allows you to know what is happening with the variable at given times. An example is didSet. Whenever the variable is set the function didSet will be called. There is also a willSet. Here is an example:
```Swift
	var nameOfMyVariable: Double = 0 {
		willSet {
			// What you want to do before the variable is set
		}
		didSet {
			// More commonly used what you want to do after the variable is set
		}
	}
```

## Pizza Delivery Example
Here is an example of a basic structure that might be used for a pizza delivery app using structs:
```Swift
	struct Order {
    	let person: Person
    	let pizza: Pizza
    	let price: Double
    	let timeOrdered: Date
	}
	struct Person {
    	let firstName: String
    	let lastName: String
	}
	struct Pizza {
    	let name: String
    	let ingredients: [Ingredient]
	}
	struct Ingredient {
    	let name: String
    	let count: Double
	}
```




