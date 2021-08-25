# Collections

## Learning Objectives
- How to declare a collection
- Name two types of collections
- How to add and remove values from a collection

## Arrays

Arrays are a way to store multiple types of the same information together. You could have a collection of strings, or a collection of doubles. Note that in arrays everything stored inside has to be of the same type.

*Declaring* an array looks like this:
```Swift
var myArray = ["Alan", "Ryan", "Ben", "Mike"]
```
This array is a collection of Strings.

*Indexes* are how arrays are ordered and stored. Each object in an array has an index. Arrays are zero based. In the example array above "Alan" is at index 0, "Ryan" is at index 1, "Ben" is at index 2, "Mike" is at index 3. The count of the array would be 4.

*Adding and Removing* objects from an array is done by using the append and remove functions. Appending an object puts the object at the end of the array. To remove an object you need to know what index to remove. Here is an example using the array from above:
```Swift
myArray.append("Nathan") // Puts "Nathan at the end of the array"
myArray.remove(at: 0) // Removes the first object in the array "Alan"
print(myArray) // Result would be: ["Ryan", "Ben", "Mike", "Nathan"]
```

## Dictionaries

Dictionaries are another collection like an array. However, in a dictionary each object has a key value pair. As well you can store multiple types of objects in the same dictionary. Dictionaries are not ordered.

*Key Value* pairs are used in dictionaries to store and retrieve information. In order to get a value out of a dictionary you need its corresponding key. 

*Declaring* a dictionary looks like this:
```Swift
var myDictionary: [String: Any] = ["name": "John", "age": 25]
```
You give it the type of [String: Any]. That means the key is going to be a String, and the value will be Any. Any meaning that is could be anything.

*Getting a value* from a dictionary is done by calling the key. It looks like this:
```Swift
myDictionary["name"] // This returns John
```

*Adding and Removing* objects from a dictionary revolve around the keys. Here is how:
```Swift
myDictionary["isMale"] = true // Adds a new key value pair of "isMale" : true
myDictionary.removeValue(forKey: "age") // Removes the key value pair of age
print(myDictionary) // Results: ["name": "John", "isMale": true]
```




