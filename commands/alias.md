---
wikiWrapper: TextArticle
---
Command: Alias.
Format:  alias &lt;command&gt; &lt;command list&gt;
         alias &lt;option&gt; &lt;arg&gt;
Example: alias km kill monster
         alias kp kill $n

     An alias is a shortened verson of a command, usually one you use
often.  When you type the alias and press return, the longer command is
executed.  An alias consists of two parts, as in the format above:
the command, and the command list that the alias is associated with.

     EotL defines some aliases for you when you create a new character.
Typing &lt;alias&gt; by itself will show you these, plus any other aliases
you have defined yourself.  Pre-defined aliases are marked with a plus (+).

-- Adding an alias:

     To set your own aliases, follow the format shown above.  Aliases
can only execute one command each.

     In the second example above, a $n is used.  These command line
arguments are denoted by '$n' where 'n' is the numbers 1 through 9,
or an asterix (*).  They represent the following:
          $1   -   the first argument.
          $2   -   the second argument, etc.
          $*   -   the remaining arguments not used by the '$n' format.
          $0   -   all off the arguments, regardless of previous use.

     Example : alias kp kill $1
     command : kp guest
     Thus    : kill guest

The following two examples show the difference between $* and $0 :

     Example : alias talk say $1 $2 $3 $*
     Command : talk a b c d e f g
     Thus    : say a b c d e f g

     Example: alias talk say $1 $2 $3 $0
     Command: talk a b c d e f g
     Thus    : say a b c a b c d e f g

-- Checking an alias.

     You can check what an alias is defined to be by typing alias &lt;command&gt;.

     For example:
          If you had 'hi' aliased to 'say hi', typing 'alias hi' would
          result in the message: 'hi' aliased to: say hi

     You can also list all the aliases with an expression in them.
     Typing 'alias -a hi' would list all the aliases with hi in them.
     
-- Checking an alias for an expression
     
     There are two ways that you can check your list of aliases for the
occurrence of a certain expression.  The -a option will check the names 
of your aliases for a certain expression, while alias -k will check
the actual alias itself.

     For example:

          If you have the following aliases defined:
               alias cha channel auction
               alias chg channel gossip
               alias kch kill chester
               alias kc  kill copland
          
          alias -a ch would return the first three while
          alias -k kill would only return the last two.
          
See also: unalias, clearaliases, expand.
