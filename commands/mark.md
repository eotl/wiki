---
wikiWrapper: TextArticle
---
Command : Mark
Format  : mark &lt;[object]|[all [id]]|[equip] [as &lt;extra&gt;]&gt;
 
     Marking an object prevents it from being sold -- handy to do with
your healing or other items that aren't worn, wielded, or held.  Objects must
be unmarked before storing.
 
     &lt;mark equip&gt; will mark all the equipment you're wearing/wielding,
&lt;mark all&gt; will mark your entire inventory, and &lt;mark all [id]&gt; will mark 
everything matching "id" (so "mark all armor" will mark all the armor in 
your inventory).

         &lt;mark item as [extra]&gt;, &lt;mark all item as [extra]&gt; will name items with an
extra identifier.  eg: 'mark fruit as HI' will mark fruit with tag (name HI).

	Once an object is named, you can then access it by using its name.
For example, If you are carrying "a backpack (named toys)", you can use the
command "drop backpack named toys" to get all the items from that pack
without confusing it with another pack.  As a shortcut, the command 
"drop named toys" would also work.
 
See also: unmark
