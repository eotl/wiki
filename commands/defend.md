---
wrapper: "../../../js/components/wiki/TextArticle"
---
Command : Defend
Format  : defend &lt;who&gt;
 
     The defend command is used to begin protecting a player from other
players or monsters.  When you are defending a person and he/she/it is
attacked, you automagically step in front and start taking hits.  If you 
just type 'defend' it will display everyone you are currently defending.
To stop defending someone, just type defend &lt;who&gt; again.

     You can set custom messages for defending in combat via the set
command.  The syntax for that is set defend-msg &lt;who&gt; &lt;what&gt;.  Where who
is the person that is going to see the message when you defend someone.
Valid values for who are: self, attacker, defendee, room.
Self is you (duh).  The attacker is the person that attacked your charge.
The defendee is your charge.  The room is everyone else.
If you wish to see what the current messages are, just type 'set defend-msg'

     You can also set colors for the first three messages via the color
command.  The syntax for that is: color &lt;who&gt; &lt;color&gt;.  Valid values for
who are: defender, defendee, defended.  Defender is you.  Defendee is the
person that got attacked.  Defended is the person you protected defendee
from.

See also: combat, color, set.
