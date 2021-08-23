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
- UILabel - Text that you can show to the user, not editable by the user

## Beginning Constraints

There are many different screen sizes and devices. Putting all of your elements onto one canvas does not mean it will look the same on all devices. To solve this we have constraints. Constraints are what keeps your views the same size and in the same position across all devices and sizes. It takes a lot of work to get them perfect. Here we will just cover some of the basics.

In order for a storyboard element to stay in the same position it needs to be anchored into that spot from all sides. If it doesn't have an anchor on what side then it will fill all the space that it can. Here are a few constraints you can use:

*leading* Anchors the view to the left side
*trailing* Anchors the view to the right side
*top* Anchors the view to the top
*bottom* Anchors the view to the bottom
*height* Makes the view always the same height
*width* Makes the view always the same width

Note we don't use left and right because in some languages it is read and used in the opposition direction. That is the reason we use the words trailing and leading. An easy way to remember is left and leading both start with the same letter.

## Outlets vs. Actions

In order to add an action or an outlet you control drag from the element in storyboard to your code. You can open Storyboard and your coding file to be side by side. To do this you can have storyboard open and option - click on the file you want to open besides it. Alternatively you can select Editor -> Assistant in the menu options.

It is recommended to add outlets above your ViewDidLoad and actions below your ViewDidLoad.

*Outlet* Outlets are used so that you can reference the element in your code. If you had a label and want to reference that label based off of an if statement you would need access in your code. Outlets let you change storyboard elements in your code.

*Action* Actions are new functions that are created. These functions are called when an action occurs. Actions include when a button is tapped, slider is moved, switch is changed, etc... Creating and IBAction in code gives you the ability to react to a users input.

## Common Missteps

Oftentimes you will create an outlet name it wrong. Delete the outlet and re-add it. The problem is when you create an outlet it adds the line of code for you, but it also adds it into storyboard. To delete the outlet in storyboard click on the element. In the right column select the right most object the "Connections Inspector" delete any unused outlets there. If you only delete the outlet in code and not in the storyboard your app will crash.






