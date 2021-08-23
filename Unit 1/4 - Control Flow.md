# Control Flow

## Learning Objectives
- Be able to explain what an if else statement is
- Use logical operators NOT, AND, and OR
- Be able to use a switch statement
- Be able to use the ternary operator

## Logical Operators

In Swift there are a list of comparison and logical operators that can be helpful in determining what chunks of code you want to run at what time.

| Operator | Type | Description |
|----------|------|-------------|
| == | Comparison | Two items must be equal |
| != | Comparison | The values must not be equal to each other |
| > | Comparison | Value on the left must be greater than the value on the right |
| >= | Comparison | Value on the left must be greater than or equal to the value on the right |
| < | Comparison | Value on the left must be less than the value on the right |
| <= | Comparison | Value on the left must be less than or equal to the value on the right |
| && | Logical | AND - The conditional statement on the left and right must be true |
| \|\| | Logical | OR - The conditional statement on the left or right must be true |
| ! | Logical | NOT - Returns the logical opposite of the conditional statement immediately following the operator |

## If Statements

An If statement is used to determine if a chunk of code should be run. In a score keeping app you may want to check if one person has a higher score than another person. If person one has a higher score you would want to display different information than if person 2 was in the lead. For scenarios like this you can use an if statement.

An If statement can be used in cooperation with operators. In your score keeping app you may need to use the comparison operators to find out which person has the highest score. Logical operators may also be used to help determine the flow of the game. 

To declare an if statement you start with the keyword *if*. Then you declare your conditional statement. Open a curly brace and a closing curly brace *{ }*. All of the code inside of the two curly braces will be in according to your conditional statement. After the closing curly brace you can declare an else statement with they keyword else and two more curly braces. The Else statement is run if the initial conditional statement fails.

Here are some examples:

```Swift
	let isTheGameOver = false

	if isTheGameOver {
		// This happens if the value is true
	} else {
		// This happens when the value is false
	}

	let personOneScore = 5
	let personTwoScore = 10

	if personOneScore == personTwoScore {
		// They have the same score, in this case nothing would happen
	} else {
		// Everything inside the else runs when the if statement fails
		print("They have the same score")
	}

	if personOneScore != personTwoScore {
		// They have different scores, in this case any code in this block would be run
		print("Someone is winning!")
	} 
	// Else statements are not required

	if personOneScore > personTwoScore {
		print("Person one is winning!")
	}

	if personOneScore >= personTwoScore {
		print("It's possible person one is winning, but they could have the same score")
	}

	if personOneScore < personTwoScore {
		print("Person two is winning")
	}

	if personOneScore <= personTwoScore {
		print("It's possible person two is willing, but they could have the same score")
	}

	let personThreeScore = 15

	if personOneScore > personTwoScore && personOneScore > personThreeScore {
		print("Person one is beating person two and three")
	}

	if personOneScore > personTwoScore || personOneScore > personThreeScore {
		print("Person one is at least beating one person, potentially both")
	}
```

## Switch Statements

A Switch statement is used when there are a lot of conditional statements. Switch statements do not have to be exhaustive, but they can be. You can switch over a number and have a case for four numbers which wouldn't cover every conditional number that could happen. In that case you would need a default case to catch all of the conditions that aren't accounted for. As well you could have conditions for the numbers using the greater than and less than to cover all possible numbers, then you would not need a default case.

To declare a switch statement you start with the *switch* keyword, then the variable that you want to switch on followed by two curly braces. In the curly braces you declare all of the cases that can happen. For a case you use the keyword *case* what the case is, then a colon. After the colon you write the code that you want to happen if that case succeeds. Repeat for all cases. If you switch statement does not cover all possible conditions then you will need a default case as well. Here is an example:
```Swift
	let numberOfWheels = 2
	switch numberOfWheels {
	case 0:
		print("You don't have any wheels")
	case 1: 
		print("Unicycle")
	case 2: 
		print("Bicycle")
	case 3:
		print("Tricycle")
	case 4:
		print("Car")
	case 5...6:
		print("Some crazy monster truck")
	case 12:
		print("Semi-Truck")
	default:
		print("That's a lot of wheels!")
	}

```

## Ternary operators

The Ternary operator is used to write more concise code. It allows you to assign a variable based off of a condition. The ternary operator is called by using the ? operator. Here is an example of how it works:
```Swift
	var largest: Int
	let a = 15
	let b = 4

	largest = a > b ? a : b

```






