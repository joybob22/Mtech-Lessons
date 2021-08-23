# Welcome To Mobile Development


## Learning Objectives

- Orient yourself with Canvas
- Learn why Swift is a great starting language
- How to use Xcode to run Swift
- Get to know your classmates


## Canvas

Canvas is a learning management tool. Everyone will be expected to be active in Canvas. All Assignments and links to extra resources can be found in Canvas.

The login to canvas is the same as your student portal. Your email is FIRSTNAME.LASTNAMEXXXX@STU.MTEC.EDU. The X's being the last four of your student ID. Your password is what you setup with you applied/registered for the program. If you are having issues in logging into canvas please contact studentservices@mtec.edu

There is an assignment in Canvas for every lab in the book. There will also be multiple quizzes per unit. These quizzes reflect the same questions that are found at the end of each lesson in the book. As well in Canvas for each lesson you can find videos, other lesson content, and next steps if you want to go above and beyond.

## Swift

When the App Store was introduced all of the apps were built in Objective-C. In 2014 Apple introduced a more modern approach to programming in Swift. In the beginning there was a lot of hesitancy to learn and use Swift. Today Swift is used worldwide. The adoption rate of Swift was rapid and by 2017 majority of new apps were written in Swift. Swift is used in all of the Apple platforms including iOS, WatchOS, TvOS, MacOS, iPadOS, and more to come.

Modern languages are safe, fast, and most of the time don't have semi-colons. As you begin to learn Swift you will start to understand how Swift has built in safety and runs relatively quickly.

These are some features of Swift:
- Clean syntax, which makes code readable and easier to work with
- Optionals, a new way of expressing when a value may not exist
- Type inference, which speeds up development and allows the compiler to help identify common issues
- Type safety, which enforces code that’s less likely to crash your program
- Automatic Reference Counting (ARC) for memory management, which automatically handles some of the deeper technical challenges of native programming
- Tuples and multiple return values, which allow smaller units of code to do more
- Generics, which help developers write code that can be used in multiple scenarios
- Fast and concise iteration over collections, making Swift a fast language
- Structs that support methods, extensions, and protocols, which allow Swift to optimize for memory use and speed while providing flexibility for developers
- Map, filter, reduce, and other functional programming patterns, which simplify code and streamline common actions that previously required multiple lines of code
- Powerful error handling, which helps the developer write fewer bugs and better handle scenarios that could cause apps to crash or perform unexpectedly

By the end of the course you can look back on this list and see everything you have learned about Swift. I would encourage you to come back and see how far you have come at the conclusion of the program

In 2015 Apple released Swift as an open source project. That means right now you can go look and see everything that makes the language. Everyone is welcome to see it as well as contribute. If there is something about Swift that you don't like you can put in a request to change it. There have been many community lead changes that have been implemented into Swift over the years. Right now a lot of it will go over your head, but as well you learn the language I would encourage you to follow along with how Swift is changing from year to year. [Swift.org](https://swift.org)

## Xcode

It's time to write your first lines of code in Swift. Xcode is an Integrated Development Environment. In simple terms that means in Xcode you can write code and Xcode will run your code and output a result.

In a few lessons we will cover a lot of what Xcode has to offer, for today we will cover a couple of the very basics. To write your first lines of code we will start with a playground. When you open Xcode you will get a couple of options of what you can start with. Select File -> New - >Playground

It's common for your first line of code to print out a statement like Hello World to the console. That is what we will do today. When you opened a playground you will see a large text editing space. This is where we will type our code. To print Hello World to the console type this line of code: 
```
	print("Hello, world!")
```
Congratulations you just wrote your first line of code. You can see the results in two places in your playground. The right column will show live updates as you type lines of Code. You can see the output "Hello, world!" there. As well if you run your code by clicking the play button by hovering over the number for the lines of code. This will run your code in the console that you can see at the bottom of the playground.


## Get to know you app

You've written your first line of code, it's time to build your first app! I want to get to know you so your task is to build an app all about you. Here is how to do it.

Open Xcode. Create a new project, File -> New -> Project -> App -> Name your project -> Choose where to save it. I'd recommend having a folder where you save all of your projects.

Once your project has been created you may be overwhelmed with all of the information, that is okay. On the left you will see a list of files. Find Main.Storyboard and select it. This will open up a canvas showing a mock iPhone. Your job is to will that iPhone canvas with things about you. To add something to the canvas click the "+" button in the top bar. You can explore your options on what you can add. I'd recommend sticking with UILabel, UITextViews, and UIImage views. You can drag and drop those elements into your canvas. Then you can click to resize them and edit their text.

In order to add an image it will take a couple of extra steps.
1. Add an imageView into your storyboard canvas
2. Google search or find a photo that you want to add
3. Open Xcode and open the Assets folder found in the left column with all the other files
4. Drag and drop your image into the assets
5. Go back to storyboard and select your imageView
6. On the right there is a new column the top option is image. Select the image you just added

Congratulations you just created your first app. You can run it in simulator and or on your phone by clicking the big play button at the top left of Xcode.


## Additional Resources

- [Mtech canvas](https://mtec.instructure.com)
- [Learn More About Swift](https://developer.apple.com/swift/)
- [Open source swift](https://github.com/apple/swift)
