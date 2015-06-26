# Introduction #
This is a sample tutorial demonstrating custom component which creates an automated, animated dropdown table view in any iphone UIView component.


# Integration steps #
  * Import QuartzCore.framework in your application.
  * Import DropDownView.h file in the view controller.
  * Have an class variable dataArray to store data to be put into the table and make a class variable of DropDownView. Making DropDownView variable allows you to control the DropDownView.
  * Use the DropDownViewDelgate and declare the delegate method in your application.
  * Initialize the DropdownView variable and add the view in your current view, andy your ready to go.
_> dropDownView = [[alloc](DropDownView.md) initWithArrayData:arrayData cellHeight:30 heightTableView:200 paddingTop:-8 paddingLeft:-5 paddingRight:-10 refView:button animation:BLENDIN openAnimationDuration:2 closeAnimationDuration:2];_

> dropDownView.delegate = self;

> [self.view addSubview:dropDownView.view];
