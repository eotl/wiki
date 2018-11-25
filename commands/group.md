---
wrapper: "../../../js/components/wiki/TextArticle"
---
Command : Group.
Format  : group &lt;subcommand&gt; &lt;arguments&gt; 
Example : group invite Duncan

-- Beginning a group:
     Any player may be in a group, simply by inviting another player to 
group with them.  The first player becomes the leader of the group.

     Leader's commands:

        group invite &lt;player&gt;   - invite &lt;player&gt; to join the group
        group leader &lt;member&gt;   - pass leadership of the group onto &lt;member&gt;
        group name &lt;name&gt;       - (re)name the group &lt;name&gt;
                                  Note: if you name your group, other
                                  people will will be able to see its
                                  membership via the 'who -o' and 'who -G'
                                  command.  Typing "group name" with no argument
                                  will un-name the group.
        group remove &lt;member&gt;   - remove &lt;member&gt; from the group

     Any member of the group may use the following commands :

        group accept            - accept an invitation to join a group
        group hp                - display each member's hp/mana/fatigue
        group leave             - leave the group you are currently in
        group status            - display information about the group
        group say &lt;message&gt;     - send &lt;message&gt; to every member in the group
        group split             - split your coins with members of the group
                                  (who must be present at the time)

     All arguments in the above commands are mandatory. 

     Typing &lt;group&gt; by itself will either display the name of the group you
are in, the name of the person / group that last invited you to join them,
or nothing.

See also: groups (for general information on how groups work)
