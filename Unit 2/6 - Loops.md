# Loops

## Learning Objectives
- How to iterate through a collection
- Know how to use a for in loop
- Know how to use a while loop

## For In Loops

Loops are used to go through every value in a collection. It gives you a chance to write a chunk of code that will run for each value. Say you had an array of people and you want to increase everyone's age by one. You could loop through the array of people and change each one. 

A for in loop is the most commonly used loop that you will use in Swift. It starts with the keyword "for", then you name a variable, keyword "in", then you declare the collection you intend to loop through, open the curly braces. The variable you created will be what gives you access to each item in the loop. If the collection had 5 items in it, the loop would run 5 times. The first time the variable would be the first item in the loop, the second time it would be the second item, and so on... Here is an example of how to use a for in loop with an array.
```Swift
let array = ["Apples", "Oranges", "Grapes"]
for fruit in array {
    print(fruit)
    // Will print three lines each with on of the fruits.
}
```

*Using Numbers* is also possible in a loop. If you want to loop over a range of numbers you can do so. Here is an example:

```Swift
for number in  1...100 {
    print(number)
    // Every number from 1 to 100 will be printed
}
```

## While Loops
Another type of loop is a while loop. These loops continue to run until a condition is met. This means the loop could run forever unless you write something to change the code. Do not write infinite loops. While loops are written by first using the "while" keyword, then writing your condition, open curly braces. Here is an example:
```Swift
var number = 10

while number < 15 {
    number += 1
    print(number) // This will print 11-15
}
```

## Control Transfer Statements
While in a loop there are some key words that you can use to help manage the state of your loop.

*Break* Break is used to exit the loop. If you use the break keyword then your loop will end and all code after the break in the loop will not be executed.

*Continue* Continue is used to go to the next item in the loop. All code after the continue will not run for the current item, but will be run for future items if the continue is not called again.

