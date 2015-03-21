### EventNotification module for Drupal ###

This module checks every day all event for notication xml tags. If found and the notication flag is not passed yet, a notication email is send.

Key features:
  * Enable email notification for upcoming events.
  * CSV event bulkload support (Event template is filled with CSV data)
  * Drupal 5.X compliant

event tag format
</event\_notification email=test@test.com >
or memberId of addressbook module
</event\_notification email=204 >

email tag content destination email address
period tag contants time in hours before email notifcation is send

Note: Crontab must run every hour.
Event mail check is only executed ones a day between 00:00 and 00:59 localtime

Checkout http://www.plaatsoft.nl for more information.

### Event Notification Feed ###
<wiki:gadget url="http://google-code-feed-gadget.googlecode.com/svn/trunk/gadget.xml" up\_feeds="http://www.plaatsoft.nl/category/eventnotification/feed/" width="780"  height="250" border="0" up\_showaddbutton="0" />