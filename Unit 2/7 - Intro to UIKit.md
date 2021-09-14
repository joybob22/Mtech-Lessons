# Intro to UIKit

## Learning Objectives
- Be able to explain the importance of UIKit
- Be able to name 5 or more views in apps
- Be able to name 5 of more controls in apps
- Be able to use segues to move around in the app

## Intro
In this lesson we will cover some of the basic views and controls. A view is something that a user is going to see and may or may not interact with. While a control is something a user has ability to interact with. Below is a breakdown of common views and controls and what they do.

## Views

*UILabel* Displays text. Can be multiple lines and as long as you need. 

*UIImageView* Displays an image. 

*UITextView* Displays multiple lines of text that can be edited by the user.

*UIScrollViews* Allows the view to scroll. Everything nested inside of the scroll view can scroll the rest of the view would not be able to.

*UITableViews* Displays a list of scroll able items. Has both static and dynamic types. Will be covered in depth in future lessons.

*UIToolBar* Displays a bar, typically at the bottom of a view. A place where you can put buttons are other controls.

*UINavigationBar* Displays a bar, always at the top. A navigation bar gives you access to back buttons. They can be customized to be different sizes, typically used by embedding in a navigation controller.

*UITabBar* Form of navigation that appears at the bottom of the screen. Allows you to be able to navigate to different portions of app from any screen. Typically there are navigation controllers for each tab, the state of navigation is saved as a user jumps around tabs.

## Controls

*UIButton* Allows a user to tap. You are able to do something when the user taps on the button.

*UISegmentedControl* Allows a user to select a value from a list of values. 

*UITextField* Allows a user to enter text. Only allowed one line.

*UISlider* Allows a user to select a value on a range by moving the selctor left and right.

*UISwitch* Allows a user to turn on or off. 

*UIDatePicker* Allows a user to select a data. The picker can be customized to display different types of days, weekly, months, and times.

## Segues

A segue is a way for you to move from one view to another view. There are many segues, but for now just worry about a push segue. You can continuously push new views on to each other using a push segue. If you want to remove a view then you need to pop. Push puts new vies on the stack of view, pop takes the top view off. In Storyboard you can create a push segue by control dragging from the object that is going to initiate the segue to the view you want to push to. Pop segue is done for you through the navigation controller.

## UIViewController

A UIViewController is your way of controlling the views on storyboard. Each view on storyboard should have a view controller file in your project. In the View Controller you can create your outlets and actions that help you manage your view's state. 

