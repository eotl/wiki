---
wrapper: "../../../js/components/wiki/TextArticle"
---
Command : Condition
Format  : condition [thing]

The condition command tells you a monster or player's current condition,
so you can get an idea of how much you (or anyone else) has damaged them.
The monster's current condition is listed in their long description, so
looking at them has a similar (although more verbose) effect.

If you do not supply a 'thing', condition will tell you the condition of
the monsters or players with whom you are engaged in combat.  Additionally,
you may specify 'me' (to check your condition) and 'all' (to check the
condition of everything living in the room).

If you have ANSI colors enabled, you can customize the color of the condition
message through the 'color' command.  Refer to its documentation for more
details.  Additionally, if the thing you are checking is in one of your
notification lists, its name will be colored accordingly.  See the
'notify' command's documentation for more information.

If there are several monsters or players in the room that respond to the
name you pass to the command, the default behaviour is to list all their
conditions.  If you are in combat, only the ones you are fighting will
be listed, generally (if only one object responds to the name you passed,
and you aren't fighting it, its condition will be listed anyway).

See also: look, consider, notify, color.
