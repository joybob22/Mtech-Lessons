# Strings

## Learning Objectives
- How to declare a string
- Know the difference between concatenation and interpolation
- Know how to compare strings

## Concatenation & Interpolation

*Concatenation* is the ability to add multiple strings together to form one bigger string. You can use the "+" operator to add two strings together. You can also use the "+=". Here is an example:
```Swift
	let firstString = "First"
	let secondString = "Second"

	let combined = firstString + secondString
	// combined value is FirstSecond, note that spaces are not added for you
```

*Interpolation* is the ability to add a string inside of another string. You can do this by using the backslash and parenthesis like this "\()". Inside the parenthesis you can add your other string. Here is an example:
```Swift
	let firstString = "First"
	let combined = "\(firstString) and Second"
	// combined value is First and Second
```

You can also do this with other data types. If you want to add a number into your string you can do something like this:
```Swift
	let age = 28
	let ageString = "I am \(age) years old"
	// ageString value is "I am 28 years old"
```

## Comparing Strings

When you are comparing two strings to see if they are the same or different punctuation and capitalization matter. If one string is capitalized and the other is not then the two strings are not the same. A helpful function you can call on strings is ".lowercased()". Here is an example:

```Swift
	let firstString = "First"
	let firstAgain = "first"

	if firstString.lowercased() == firstAgain {
		// This code would succeed because each string is lowercased.
	}
```

## Common functions

Here are a bunch of functions and other topics that are used in Strings. There are a lot more that you can check out in the documentation but this is a start.

| Function | Description |
|---------|-------------|
|lowercased() | takes all of the characters in a string and makes them lower case|
|uppercased()| takes all of the character in a string and makes them upper case|
|contains() | checks to see if a string contains whatever variable you pass in|
|remove(at:)| Removes chracters from your string|
|firstIndex(of:)| First time the variable appears in the string|
|count| Returns how many chracters are in the string|
|isEmpty| Returns a Bool is your string is empty or not|
|append()| Appends the given string to a this string|

## Emojis

You can add emojis into your string as well as make them variable names. I would not recommend using emojis for your variable names. To open to emoji keyboard the shortcut is Control->Command->Space. Emojis count as one character in a string.
