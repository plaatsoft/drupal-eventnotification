Created by wplaat (Plaatsoft)

This software is open source and may be copied, distributed or modified under the terms of the GNU General Public License (GPL) Version 2
 
For more information visit the following website.
Website : http://www.plaatsoft.nl 
 
Or send an email to the following address.
Email   : info@plaatsoft.nl

General
-------
This module is check every day all event for notication xml tags. If found and notication flag is not passed yet notication email is send.

event tag format
</event_notification email=wvdp@bigfoot.com >
 or memberId of addressbook module
</event_notification email=204 >

email tag content destination email address
period tag contants time in hours before email notifcation is send

Note: Crontab must run every hour.
Event mail check is only executed ones a day between 00:00 and 00:59 localtime

Key features
------------
 - Enable email notification for events.

 - Upload bulk events with email notification
 - CSV format
   Date;info_block1;Time;Name1_block2;Name2_block2;Name3_block2;Name4_block2;Name5_block2;Name6_block2;;Name1_block3;Name2_block3;Name3_block3;;

   Example:
   11-10-2009;;9:00;Hester Gijsbertsen;Annette Abrahamse;;Ingrid Roosendaal;Micha Kastelein;Annemarieke Brak;;Mieke Reijersen van Buuren;Andrea Kerssen;;

Requirements
------------
This module requires the latest development version 5.1 or 4.7 of Drupal (CVS HEAD).
And the GD library must be active in the php apache module else images will not work!

Installation
------------

1. Copy the event_notificator folder and its contents to the Drupal modules/ directory. 
   Drupal should automatically detect it and create nessary database queries.

2. Go to 'administer -> modules' and enable event_notificator.
 
3. Configure the module
 
   http://!your URL!/admin/settings/event_notification

4. Optional: To upload a bulk events use the following link.
   http://!your URL!/event_notification
 
Release Notes
-------------
 
History:

10-10-2007  v1.0
- Created

30-03-2008  v1.1
- Add addresbook email lookup

27-04-2008  v1.2
- Add variable sender email address in configuration 

20-07-2008  v1.3
- Add CSV upload functionality

18-01-2009  v2.0
- Improve documentation.

15-09-2009  v2.1
- Improve version tag of module
- First release on drupal.org
- First official release for drupal.org

16-09-2009  v2.2
- BugFix: Now auto module upgrade detection is working.
- Updated drupal.org event_notification cvs repository for automatic update detection.

10-10-2009  v2.3
- Adapted CSV conver functionality to be compliant with new CSV format.
 
Known Minor Issues
------------------
- None
 
Nice to have
------------
- None
