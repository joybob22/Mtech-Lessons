# Documentation

## Learning Objectives
- How to use the documentation browser
- How to find sample code and framework guides

## Using Apple Documentation

Every framework that Apple provides has documentation behind it. Documentation is what Apple gives you to help you understand how everything inside of the framework works. Documentation is not just from Apple, if you are using any type of third party framework they should also provide documentation. A lot of the time when you're looking for new third party frameworks you can look at their documentation to see if it is worth your time or not.

## Using Quick Help

Any code that you write that is colored you can click on to find the documentation for it. Even the own code you write, you can write documentation for all of your own code as well. Today is focused on the documentation from Apple.

Opening any of your projects going into a viewController we can see a couple of colored items in your code. When you declare the class there is the UIViewController.
```Swift
	class ViewController: UIViewController
```
In order to see the documentation for what a UIViewController is there are a couple of shortcuts. 
| Command | Description |
|---------|-------------|
|Option - click | Shows quick help, gives an introduction|
|Command - click | Shows a menu of options to choose from|
|Shift - Command - 0 | Opens the documentation window|

When you option-click to show the quick help you get an option at the bottom to open in Apple Documentation. That will open up to give you the full details of what you clicked on. 

When you command-click you get the option to show quick help, you can also see what other pieces of code call what you clicked on, edit that piece of code everywhere, and lastly you can jump to definition. Jumping to definition takes you to a new screen to where you can see the code that Apple wrote to support this framework. This screen can be a bit overwhelming, but can show a lot of information that you wouldn't get elsewhere.

Another way to open the documentation is Shift - Command - 0. Also accessible by going to Window -> Developer Documentation. You can then search in this documentation window to find whatever you are looking for.

## Reading Apple Documentation

Apple Documentation is broken up into a couple of pieces. 

*Declaration* This is how to name and access the property

*Overview* A breakdown of how it is used. More common topics will have a larger overview giving a quick lesson on how it works.

*Discussion* In-depth description going into all of the details of the selected subject

*Availability* What iOS it is available in

*Framework* What framework you need to import in order to use the selected subject

*Topics* Related items that may be helpful to your selected subject

## Effective Googling

People that learn how to code quickly are often the same people that know how to google what they are looking for. Googling is a tool that will save you a lot of time. Here will be shown a couple of ways that you can increase your skill in finding the answer in google.

### Writing your search query

When writing your search query think about how someone with the answer to your problem would phrase your question. Don't use terms that are specific to your project. If you're writing a score keeping app and need to know how to display the score. Instead of writing your query like "How to show score text" you could make it more generic and say "How to show label with custom text". Majority of all your questions and answers to your problems are on the internet. You just have to find them.

Here are a list of useful tools in google searches:
| Command | Description |
|---------|-------------|
|Put a word/phrase in quotes | Search for the phrase exactly as you have it inside the quotes. |
|Hyphen before a word| Excludes the word from your search results|
|.. | Search a range of numbers|
|OR | Search two phrases|
|related: | Find a similar site|
|* | Placeholder when you don't know what to put|

In the end just keep it simple. If the results aren't helpful then keep adding new terms.

Lastly add swift to the end of your search query. A lot of questions you may have will be relevant in many languages so it's good to add "swift" at the end to narrow down to just swift related topics.

### Finding the right result

To find the right result you need to skim. If you look at each result with a magnifying glass trying to determine if it is the right one you will be looking for far too long. Skim over the results and try to find one that is helpful to you. It is also helpful to look at the websites. As your searching skills get more adept you will find sites that you like more than others.

For me my order of preference when it comes to websites is something like the following:
1. Apple Documentation
- Always best to go straight to the source
2. Hacking with Swift
- Really helpful site. The guy that maintains it is up to date and has written a lot of great resources
3. Stack Overflow
- Your question has been asked here. Finding the right question and the answer can be challenging.
4. Tutorial sites
- The answer to your question can most likely be found in a tutorial, but they are hard to navigate and hard to find exactly what you are looking for.





