---
wikiWrapper: TextArticle
---
Command : History.
Format  : history

This command will dump out the history information for your current
login.  The format will be similar to the following:

    History List (2 Commands Total):
       1    glance
       2    history
       3    ls /bin

Up to 20 commands will be stored in your history buffer.  You can 
access these history commands by using the following command line options:

   Command         Action

    #!             Performs the last executed command.
    #$             Performs the last word of the last executed command.
    #&lt;num&gt;         Runs history command &lt;num&gt;
    #&lt;string&gt;      Runs last history command starting with &lt;string&gt;

Here are some examples using the history listed above:

    #h             history
    #1             glance
    #!             ls /bin
    #$             /bin
