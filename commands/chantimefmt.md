---
wrapper: "../../../js/components/wiki/TextArticle"
---
Command: Chantimefmt
Format : set chantimefmt &lt;format&gt;

     This allows a player to control the format of channel
message timestamps.  The setting is a format string passed
to strftime.  Below are the possibilities:

         %%    same as %
         %A    locale's full weekday name
         %a    locale's abbreviated weekday name
         %B    locale's full month name
         %b    locale's abbreviated month name
         %c    locale's appropriate date and time representation
         %C    same as ctime(tyme)
         %d    day of month ( 01 - 31 )
         %D    date as %m/%d/%y
         %e    day of month ( 1 - 31; single digits are preceded by a blank )
         %H    hour ( 00 - 23 )
         %I    hour ( 01 - 12 )
         %k    hour ( 0 - 23; single digits are preceded by a blank )
         %l    hour ( 1 - 12; single digits are preceded by a blank )
         %m    month number ( 01 - 12 )
         %M    minute ( 00 - 59 )
         %n    same as new-line
         %p    locale's equivalent of either AM or PM
         %r    time as %I:%M:%S [AM|PM]
         %R    time as %H:%M
         %S    seconds ( 00 - 61 ), allows for leap seconds
         %t    same as a tab
         %T    time as %H:%M:%S
         %w    weekday number ( 0 - 6 ), Sunday = 0
         %x    locale's appropriate date representation
         %X    locale's appropriate time representation
         %y    year within century ( 00 - 99 )
         %Y    year as ccyy ( e.g. 1986)

Examples:
     1.  set chantimefmt %T %D

         02:03:36 03/31/96 &lt;Channel&gt; Bert: hi!

     2.  set chantimefmt %H:%M:%S

         02:03:36 &lt;Channel&gt; Bert: hi!

     3.  set chantimefmt %a-%T
         Tue-02:03:36 &lt;Channel&gt; Bert: hi!
	(this one is the default)

See also: set, chantimes

