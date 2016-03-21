# magento-php7-totals-fix
## Abstract
Here's a magento module to solve magento issues with totals calculation for php7.
The issues I've experienced in particular were that taxes have been added twice to the grand total for [pay with amazon](https://www.magentocommerce.com/magento-connect/login-and-pay-with-amazon-advanced-payment-apis-for-europe.html) module on the amazonpayments checkout page.
  
## Credits
The solution was provided by [archigrafix](http://magento.stackexchange.com/users/34992/archigrafix) on http://magento.stackexchange.com/a/97107/35665 - So this is simply the fix packed into a module.

## Background
 PHP7 has a new implementation of uasort algorithm which may behave differently for sorting elements with identical order.
 
### Further references:
http://magento.stackexchange.com/questions/92783/magento-grand-total-without-taxes-in-1-9-with-php7
http://stackoverflow.com/questions/34281113/the-different-behavior-of-the-function-uasort-in-php-5-5-and-php-7-0
http://stackoverflow.com/questions/9194281/sort-algorithm-magento-checkout-totals-sorted-wrongly-causing-wrong-shipping-ta

 
## Install
Install manually or via [modman](https://github.com/colinmollenhour/modman)...

*Note: Tested and working with Magento CE 1.9.2.1* 

