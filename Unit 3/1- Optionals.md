# Optionals

## Learning Objectives
 - Create a variable that is optional
 - Be able to unwrap an optional
 - Be able to pass optionals and return optionals from functions
 - Define a failable init
 - Know when it is okay to use the bang operator

## What's an optional

Variables and constants in your code may not always have a value. When there is no value that means the variable has a nil value. Nil means that there is nothing there. Optionals in Swift are used to work with nil values in your variables. When a variable is optional that means it may or may not have a value. If you had a person struct, you would likely have variables of name, age, and maybe occupation. Every person created will have a name and age, but not everyone will have an occupation. In this case occupation can be an optional meaning that it could have a nil value. To make a variable optional we use the "?" operator. Here is an example:
```Swift
struct Person {
	let name: String
	let age: Int
	let occupation: String?
}
```

## Unwrapping

When working with optionals it's important to know if the variable is nil or not. To check to see if the variable has value we can unwrap the optional to see what's inside. To do so we can use if-let syntax to unwrap an optional. Here is an example:
```Swift
let person = Person(name: "Joe", age: 38, occupation: "Recruiter")

print(person.occupation) // value is Optional("Recruiter")

//Unwrap the person's occupation
if let occupation = person.occupation {
	print(occupation) // value is "Recruiter"
} else {
	// Happens if the value of person.occupation is nil
}
```
Let's bread down the syntax of unwrapping an optional. It starts with an "if". After the "if" you declare a new constant that the value of the optional will be stored. In the case above the variable occupation will hold the value of what is inside the optional. After declaring the variable set it equal to the optional you are trying to unwrap. If there is a value in the optional then inside the first curly braces you will have access to that value that is captured in the variable you created in the first line. You can also still have an else statement, although that is not common when upwrapping optionals. This is the most common way to unwrap an optional and you will write hundreds of if-let statements in this class. 

## Optional Chaining

Sometimes inside of one optional you can have more optionals. Here is a data model of an example of this:
```Swift
struct House {
	let livingRoom: Room?
}
struct Room {
	let windows: Int?
}
let room = Room(windows: 5)
let house = House(livingRoom: room)
```
Here the house has an optional living room variable which is of type Room. The Room struct has an optional variable of windows. A house may or may not have a living room, and a living room may or may not have windows. If we wanted to get the number of windows we would have to unwrap the living room, then unwrap windows. Alternatively we can use optional chaining. Here is an example:
```Swift
if let windows = house.room?.windows {
	// access to windows without writing the if-let for room
}
```

## Optionals in everything
You will use optionals all the time. To start it will be annoying, but it will be useful in the long run. To continue with optionals they can be used in functions and return types. Here is how:
```Swift
func fullName(firstName: String, middleName: String?, lastName: String) -> String? {
	// middleName is optional
	// The return type will also be optional
}
```
Calling this function returns an optional, meaning you can return nil. Also means that if you call this function you would need to unwrap the value.
Middle name is also optional as a parameter in the function. That means you can pass nil into the function instead of a value.

## Failable initializer
Another use of optionals is in the initializers for your structs and classes. So far all of the inits have been returning a value no matter what. You can write a failable init that allows you to return nil instead of an object. Here is an example:
```Swift
class Person {
	let firstName: String
	let middleName: String?
	let lastName: String

	init?(firstName: String, let middleName: String?, let lastName: String) {
		if let middleName = middleName {
			self.firstName = firstName
			self.middleName = middleName
			self.lastName = lastName
		} else { 
			return nil
		}
	}
}
```
The "?" after init means it is a failable init. In this case the initializer takes an optional variable for middleName. If there is a value it creates a Person object that sets all of the variables. If there is no middle name in this case no object is created, instead it just created a nil object.

## Bang Operator
Perhaps there is a time in your code that you are 100% certain that a variable has a value and you do not want to unwrap it. To unwrap it you can use the bang operator "!". You can do this by putting an exclamation after the optional variable. This will force unwrap the variable. For this class you are not allowed to use the bang operator unless given permission. It is bad practice to use the bang operator and should be used rarely to never.



