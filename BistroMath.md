BistroMath is a specialized calculator for solving "bistromatic" problems which involve numbers on a a waiters check-pad and people in restaurants.

Given the amount on the bill, we can quickly calculate tax, tip, how to divide equally among N people or convert into another currency.

## Revision History ##
### 1.0.3 ([download](http://android-labs.googlecode.com/files/BistroMath.1.0.3.apk)) ###
  * add online help text
  * remove menu item to invoke calculator app

## 1.0.1 ([download](http://android-labs.googlecode.com/files/BistroMath.apk)) ##
  * Initial release

## Example ##
![http://android-labs.googlecode.com/svn/trunk/screenshots/bistromath1.png](http://android-labs.googlecode.com/svn/trunk/screenshots/bistromath1.png)

The goal is to be as quick and efficient as possible. In a standard case, to calculate the amount to be payed on a check of 100, this would mean - launch the BistroMath application, tap directly on the on-screen virtual keypad '1' - '0' - '0' and read the result! No fumbling with the keyboard or navigating multiple screens or dialogs.


## Changing Inputs ##
![http://android-labs.googlecode.com/svn/trunk/screenshots/bistromath2.png](http://android-labs.googlecode.com/svn/trunk/screenshots/bistromath2.png)

If any of the other input parameters are not set correctly, adjust them by selecting which field to update by menu or touch-screen and use the keypad to enter a new value. All other fields will again instantly update themselves. Fields which currently are not applicable are hidden in the display - to enter a value, select it using the menu option.

The inputable fields are (select from menu or tap on screen to modify):\n
  * Price: total amount of restaurant bill (pre or post tax depending on the situation)
  * Tax: tax rate applied to price\n
  * Tip: tipping rate applied to price\n
  * Split: number of people among which to divide the bill equally\n
  * FX Rate: currency conversion rate between the local currency of the restaurant and the users own currency in case of international travel.

![http://android-labs.googlecode.com/svn/trunk/screenshots/bistromath3.png](http://android-labs.googlecode.com/svn/trunk/screenshots/bistromath3.png)

See display fields for "Total" or "Per Person" amount for how much should be paid based on the above input.

## Before or after tax? ##
Depending on local custom or you preference, you can calculate tip before or after tax. By setting a tax rate (menu->Tax and enter the tax rate number) and a tipping rate (menu->Tip and enter the desired percentage for the tip), both values are now calculated separately based on the pre-tax amount of the bill.

For more updates, see Android related entries on my [blog](http://blog.kugelfish.com/search/label/Android)