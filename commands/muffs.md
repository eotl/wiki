---
wikiWrapper: TextArticle
---
Command : Muffs
Format  : muffs || muffs &lt;command&gt;


    This command is designed to help you block out players that you
do not wish to talk to. Use these commands to set up your muffs and
then the muffs will check tells and emotes as they come to you and
block them if nessasary.

    These muffs will not block wizards.

muffs
    Lists all your muffs settings.

muffs m
    Display your current muffs message.

muffs m &lt;msg&gt;
    Sets your muffs message to &lt;msg&gt;.
    This message will be used when someone who is in a group that you
    are blocking or screening talks to you or emotes to you. They will
    then get the message.

**Settings for the muffs are:

  off
    Lets the message through with no muffs message to the sender.

  screen
    Displays the muffs message to the sender and appears not to get
    through to the target. The target receives the message in the
    format:
    (Muffled) &lt;message&gt;

  block
    Displays the muffs message to the sender and appears not to get
    through to the target. The target does not receive the message
    at all.

**Setting the muffs:

muffs c
    This setting is linked to the player body notifier (help notify).
    This will list all your muffs settings for the categories in your
    notify list.
muffs c &lt;category&gt; &lt;setting&gt;
    Sets the muffs to &lt;setting&gt; for that &lt;category&gt;
    e.g. muffs c friends screen
    This example would mean that anyone in your notify friends
    category who sends you a message will be screened as specified
    above.

muffs eval
    Tells you the settings for the eval you are blocking. This muffs
    setting will be effective on players who are not on your notify
    list and are BELOW (not the same eval, at a lower eval only) the
    eval that you specify.
muffs eval &lt;number&gt; &lt;setting&gt;
    Sets the muffs setting for players below &lt;number&gt; eval.
    e.g. muffs eval 2 block
    This will block anyone below eval 2 who trys to send you a
    message.

muffs else
    Tells you the muffs setting for all those players who are not on
    your notify list and are above or equal to the specified eval.
muffs else &lt;setting&gt;
    Muffs will be set to &lt;setting&gt; for anyone not on notify list or
    below eval setting.

muffs RESET
    Will turn off all settings and delete your muffs message.
