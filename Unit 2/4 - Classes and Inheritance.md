# Classes and Inheritance

## Learning Objectives

- How to create a class
- Be able to describe what reference type means
- Difference between structs and classes
- How to use inheritance

## Declaring a class
Classes are very similar to structs. Classes require initializers and are reference type. That means every time a class is declared an init is required. To create an init it's a lot like a function. Start with the "init" then open parenthesis with your parameter names and types. Open curly braces. Inside the curly braces all of the variables of the class have to be set. Here is an example:

```Swift
class Person {
    let name: String
    var age: Int
    
    init(name: String, age: Int) {
        self.name = name
        self.age = age
    }
}
```

## Reference type
Classes are a reference type. That means when a class is copied it will refer back to the original copy. So if the original copy changes the new copy will change with it. Here is an example using the class above:
```Swift
var firstPerson = Person(name: "Aaron", age: 40)
let secondPerson = firstPerson
firstPerson.age += 1
print(firstPerson.age) // prints 41
print(secondPerson.age) // prints 41
```

## Inheritance
What makes classes powerful is that they can inherit from each other. You can have a parent class and a child class. The child class gets all of the functionality from the parent class as well as its own unique functionality. Here is an example:

```Swift
class ParentalUnit {
    let name: String
    let isBald: Bool
    init(name: String, isBald: Bool) {
        self.name = name
        self.isBald = isBald
    }
}
class Child: ParentalUnit {
    let personality: String
    init(personality: String, name: String, isBald: Bool) {
        super.init(name: name, isBald: isBald)
        self.personality = personality
    }
}
```
Note that when you are declaring the init for the child class you have to also pass in all of the information that you would need to create the parent class. This is done by using the super.init as seen above.

## Structs vs. Classes
- Classes are reference type
- Structs are value type
- Classes require init
- Structs do not require init
- Both are blueprints of objects

