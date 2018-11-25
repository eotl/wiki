---
wrapper: "../../../js/components/wiki/TextArticle"
---
Command : Notify
Format  : notify || notify &lt;command&gt;

     The notify command controls the login/logout notification 
inside your player body.  The different commands are as follows:

notify
  Lists your categories.

notify &lt;on/off&gt;
  Turns on/off notification.

notify &lt;on/off&gt; &lt;category&gt;
  Turns notification on/off for &lt;category&gt;. (default is on)
  
notify level &lt;level&gt;
  Sets your notification to watch for level &lt;level&gt; and above.
  &lt;level&gt; can be a string (e.g. "wizard", "frob") or an ordinal
  value.  (0 is Mortal, 1 is Guest, 2 is Frob)  You will then be
  notified of everyone ranked &lt;level&gt; and above, whether they are
  on your list or not.  Set &lt;level&gt; to 6 to turn off level notification.
  
notify beep &lt;category&gt; &lt;on/off&gt;
  Marks a notification category for beeping.

notify  &lt;category&gt;
  Lists the contents of &lt;category&gt;.

notify +c &lt;category&gt;
  Adds &lt;category&gt; to your notify list.

notify -c &lt;category&gt;
  Deletes &lt;category&gt; from your notify list.

notify +n &lt;category&gt; &lt;name&gt;
  Adds &lt;name&gt; to &lt;category&gt;.

notify -n &lt;category&gt; &lt;name&gt;
  Deletes &lt;name&gt; from &lt;category&gt;.

notify -n &lt;name&gt;
  Deletes &lt;name&gt; from your notify list.

notify color &lt;category&gt; &lt;color&gt;
  Changes the color of &lt;category&gt; to &lt;color&gt;

  Colors:
    black
    blue
    green
    cyan
    red
    purple or magenta
    yellow or brown
    white
  Modifiers:
    bold
    blink
  ( bold &lt;color&gt; can be abbreviated by adding "h" or "b" to the
    beginning of the color.  ( "bold white" becomes "bwhite" ) )

notify convert &lt;bw|bw2|gen|iff&gt;
  Temporary command for converting other friends and foes lists to
  this one.
       bw  - Converts from Binford Wiztoy
       bw2 - Converts from Binford Wiztoy Mark II
       gen - Converts from the Gentool
       iff - Converts from the SuperIFF

notify RESET
  Resets your friends/foes list to the default.

notify *check
  Fixes some problems you might be having with ansi who.
 
notify move on/off
  Sets movement notification on or off.
 
notify move on/off &lt;category&gt;
  Sets movement notification on or off for that category.
 
notify move entrance/exit
  Shows current status for default entrance or exit messagees.
 
notify move entrance/exit &lt;color&gt;
  Sets default entrance or exit message color.
 
notify move entrance/exit off
  Turns off default entrance or exit message.
