---
wrapper: "../../../js/components/wiki/TextArticle"
---
 ______________________________               ____________________________ 
|            Name              |             |          Syntax            |
|------------------------------|             |----------------------------|
| who - list on-line player(s) |             |  who [-option(s)]          |
|______________________________|             |  who [-option(s)] <player> |
                                             |____________________________|

 _________________________________________________________________________ 
|                                Description                              |
|-------------------------------------------------------------------------|
|      This command with no name specified will produce a list of the     |
|  players and wizards on-line.  For more detailed information on a       |
|  player or wizard, type 'who <name>', where <name> is the name of a     |
|  player or wizard.                                                      |
|_________________________________________________________________________|

 _________________________________________________________________________
|                                  Options                                |
|-------------------------------------------------------------------------|
|                                                                         |
|   -p          Displays people online with more detail.                  |
|               (similar to "who -p <player>")                            |
|                                                                         |
|   -p <player> Displays compressed info on a player.                     |
|               (see explanation below)                                   |
|                                                                         |
|   -l <group>  Displays laston information for a group of people in      |
|               your notify list.                                         |
|                                                                         |
|   -l <player> Displays laston information for a person.                 |
|                                                                         |
|   -c          Displays people online in your notification list.         |
|               (like chum -s in the iff)                                 |
|                                                                         |
|   -e          Displays people online who have you in a notification     |
|               list.                                                     |
|                                                                         |
|   -n          Displays people online in your notification list along    |
|               with the notify category they are in.                     |
|                                                                         |
|   -o          Displays people online by their short description.        |
|               (old who)                                                 |
|                                                                         |
|   -i <player> Displays miscellaneous player info on a person.           |
|               (like the gentool's "[info <player>")                     |
|                                                                         |
|   -w          Wizard list - lists only wizards.                         |
|                                                                         |
|   -m          Mortal list - lists only mortals.                         |
|                                                                         |
|   -g          Lists players and wizards separated by guild name.        |
|                                                                         |
|   -G          Lists players and wizards separated by group name.        |
|                                                                         |
|   -r          Lists players and wizards separated by race.              |
|                                                                         |
|   -s <sort>   Lists players, sorted by the specified sort               |
|               <sort> can be one of the following:                       |
|                 eval      age       level (default)                     |
|                 guild     gender    specialization                      |
|                 race                                                    |
|                                                                         |
|   -f <filter> Lists all players that match the filter.                  |
|               They can be stacked for narrower output.                  |
|               <filter> can be one of the following:                     |
|                 high-eval  low-eval  mid-eval                           |
|                 g:<guild>  r:<race>  e:<gender>                         |
|                 wizard     mortal    i:time                             |
|               Where <guild>, <race>, and <gender> are                   |
|               regular expressions.                                      |
|               i:3600 would show anyone under an hour idle               |
|               i:<3600 also shows anyone under an hour idle              |
|               i:>3600 would show anyone over an hour idle               |
|                                                                         |
|   -b <player> Like who <player>, but inserts page breaks.               |
|                                                                         |
|   -F <player> Like who <player>, but displays one's finger-plan.  Works |
|               only for wizards; otherwise, it's the same as             |
|               who <player>.                                             |
|                                                                         |
|   -C Lists people on notify lists (like -c) with format of -w           |
|                                                                         |
|   -W Lists anyone who is either on a notify list, an immortal, or both. |
|      Uses -w format.                                                    |
|_________________________________________________________________________|
 __________________________               ________________________________ 
|        Evaluation        |             |              Age               |
|  Title          Range    |             |  Title           Range (days)  |
|--------------------------|             |--------------------------------|
|  Insect         1-5      |             |  Newborn         0             |
|  Newbie         6-12     |             |  Kid             1-2           |
|  Novice         13-25    |             |  Teen            3-4           |
|  Average        26-45    |             |  Young adult     5-8           |
|  Better         46-55    |             |  Adult           9-14          |
|  Skilled        56-65    |             |  Gettin' on      15-20         |
|  Advanced       66-75    |             |  Old Fart        21-30         |
|  Expert         76-85    |             |  Ancient         31-50         |
|  Master         86-92    |             |  Ageless         51-100        |
|  Terrific       93-100   |             |  > Ageless?      101-150       |
|  Awesome        101-110  |             |  Oh My           151-200       |
|  Radical        111-120  |             |  Ladylunar?      201+          |
|  Coolness       121-130  |             |________________________________|
|  Wow!           131-150  |
|  Ugh            151-160  |
|  Bleah          161-199  |
|  Insane         200+     |
|__________________________|

A '#' by someone's name indicates that that person is currently in the
editor.  Only those of immortal rank should have this by their names;
if they do, do not bother them.


who -p <name> explained:

                 Linkdead   Idle:seconds  Online/Laston:time
                      \           \         /
  ____________________________________________________________________________
 | [Wiz] Devo        |LD|ED|M:2  |I:30  |O:26m |G:Fighter     |S:Swordsman    |
  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
      |                  /    \                      |              |
     Name            Editing  Mail:new letters     Guild        Specialization


   Jimmy Wolf sez, "who.c: It's not crap anymore!"
  
                  ( It's not crap anymore! )
   |\   /|       O
    o   o    o
      0    .
    |_|_|
   | |_| |


 _________________________________________  
|  See also 'anonymous' and 'evaluation'  |
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
