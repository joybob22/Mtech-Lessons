# Interface Builder

## Learning Objectives
- How to add new elements to a storyboard
- How to add constraints
- Know the difference between an outlet and actions

## Common UIKit Elements

When in storyboard in the top right there is a "+" button. You can use this button to drag and drop new elements into your screens. The most common elements are these:

- UIButton - used for selecting something
- UITextView - used for long form text entry. Can be multiple lines
- UITextField - used for short form text entry. Only one line
- UISlider - used to show progress or a range
- UISwitch - used to show off and on
- UILabel - Text that you can show to the user, not edittable by the user

## Beginning Constraints

## Outlets vs. Actions

In order to add an action or an outlet you control drag from the element in storyboard to your code. You can open Storyboard and your coding file to be side by side. To do this you can have storyboard open and option - click on the file you want to open besides it. Alternatively you can select Editor -> Assistant in the menu options.

It is recommended to add outlets above your ViewDidLoad and actions below your ViewDidLoad.

*Outlet* Outlets are used so that you can reference the element in your code. If you had a label and want to reference that label based off of an if statement you would need access in your code. Outlets let you change storyboard elements in your code.

*Action* Actions are new functions that are created. These functions are called when an action occurs. Actions include when a button is tapped, slider is moved, switch is changed, etc... Creating and IBAction in code gives you the ability to react to a users input.

## Common Missteps

Oftentimes you will create an outlet name it wrong. Delete the outlet and re-add it. The problem is when you create an outlet it adds the line of code for you, but it also adds it into storyboard. To delete the outlet in storyboard click on the element. In the right column select the right most object the "Connections Inspector" delete any unused outlets there. If you only delete the outlet in code and not in the storyboard your app will crash.






