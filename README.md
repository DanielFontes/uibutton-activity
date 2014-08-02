uibutton-activity
=================

UIButton that displays an activity indicator when disabled.

Demo
====

The demo/ folder contains a demo project showing UIButton+Activity in use. Open and run it.

Usage
=====

Import "UIButton+Activity.h". Then, on any button you want to show an activity indicator when disabled, call

	[_button useActivityIndicator:YES];

The activity indicator usually works best if you also set up the button to hide its title in the disabled state:

	[_button setTitle:@"" forState:UIControlStateDisabled];

Then, to show the activity indicator, just disable the button as normal:
	
	_button.enabled = NO;

Compatibility
=============

This class has been tested back to iOS 6.0.

Implementation
==============

This class is implemented by hiding and showing a UIActivityIndicator subview when the button's enabledness changes.

License
=======

This code is released under the MIT License. See the LICENSE file for details.
