This code is for zen cart 1.58A with php 8.1. FIles are based on zen cart 2.01. 

ipn_main_handler.php no changes. <br>
paypaldp.php some changes<br>
paypalwpp.php some changes

Some key notes:

1. convertToLocalTimeZone() function will trigger warnings under zen cart 1.58A. Changed the code back to the previous version.
2. In the past updates, $order_amount is changed to $order->info['total']. Not sure if it also works under zen cart 1.58A or not.
3. With paypaldp.php (credit card processing), order confirmation will show auth code as n/a on the top. While in the previous zen cart, auth code is hidden. Updated the code to hide this n/a.

copyright @zencart
https://github.com/zencart/zencart
