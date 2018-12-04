---
wikiWrapper: TextArticle
---
Command : Nickname Substitution.
Format  : sub &lt;word&gt; &lt;meaning&gt;

   Just as aliases let you give another name to actions, subs let
you give an alternate name to objects and everything else.  When you
assign a meaning to a particular word, any use of that word will be
translated to its new meaning.  For instance, if you

   sub lite lightning

then the following lines become

   tell lite hello!            --&gt; tell lightning hello!
   give sword to lite          --&gt; give sword to lightning
   say lite up my life         --&gt; say lightning up my life

Combined with aliases, subs could save a lot of keystrokes:

   alias g get $1 from $2
   sub a all
   sub b bag
   sub c corpse

   g a b      --&gt; get all from bag
   g a c      --&gt; get all from corpse

Typing 'sub' alone without arguments will list all the subs
you have defined.  To remove a sub, use the 'unsub' command.
You can use up to 50 subs to redefine your favorite annoying
words, but you are not allowed to turn these words into subs:
sub, unsub, alias, and unalias.

   Nickname substitution only works on a word with spaces before and
after it.  Using the above example,

   big b       --&gt; big bag
   big -b      --&gt; big-b
   'hi lite!   --&gt; say hi lite!

If you want to use a word literally but it has been subd, put a
backslash (\) in front of the word.

   big \b                   --&gt; big b
   say \lite up my life     --&gt; say lite up my life

If you want to see the result of your input after aliases and subs
have been substituted, you can 'set expand on'.

   Hint #1:  don't sub 'me' into your own name, it will make all
of your spoken words sound like third person.

   Hint #2:  if you're really strapped for aliases, subs can act
as simply aliases that don't do argument substitutions.  For instance,

   sub x look at

   x dog         --&gt; look at dog

But be warned that although you can sub a command, you can't make
a sub of an alias, because subs are substituted after the
aliases.

   alias gafc get all from corpse
   sub g gafc

   g              --&gt; gafc

   Hint #3:  although subs only work when the word is separated
by spaces, the 'tell' command has been designed to accept your
subs when you use multitell.

   alias t tell
   sub l lightning
   sub n nightswimmer
   sub w windrunner

   t l, n, w huba!   --&gt; tell lightning, nightswimmer, windrunner huba!

   Hint #4:  you can also use the alias sub and unsub instead of using
sub or unsub.  If you don't have it aliased, then you can type:

   alias sub sub
   alias unsub unsub

See also:  unsub, set, expand, alias
