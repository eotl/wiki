---
wikiWrapper: TextArticle
---
Command : Wimpy Direction
Format  : wimpydir &lt;direction&gt; || wimpydir random
Example : wimpydir east

     If your player has a wimpy value set (not zero) then you may also
specify a default direction for your player to attempt to flee in, should 
wimpy be called.  Should you not have any preference, the direction
may be set to 'random'.

**NOTE**
     Wimpydir does NOT recognize aliases.  In other words, "wimpydir w" 
will NOT work to set your wimpy direction to west.  You must type the full
name of the direction, such as "wimpydir west", if you want wimpydir to 
work properly. 

See also: wimpy, set
