---
wikiWrapper: TextArticle
---
Command : Findemote.
Format  : findemote &lt;regex&gt;
          findemote -s &lt;string&gt;
Example : findemote happy

Lists all emotes (feelings) via a regular expression (regex).  Unlike 
feelings &lt;pattern&gt;, this command searches the feeling data.

The -s option (added 960614) allows players to search for a simple sub-string
instead of by regex.  This may be useful in doing things like:

findemote -s [tm]

Since [] are characters important to the regex pattern, findemote [tm] would
not work.

See also: feelings
