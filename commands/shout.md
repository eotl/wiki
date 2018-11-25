---
wrapper: "../../../js/components/wiki/TextArticle"
---
Command : shout
Format  : shout &lt;msg&gt;
          shout -d &lt;name&gt;
          shout -a &lt;name&gt;
          shout -l
          shout /last [&lt;num&gt;]
          shout /hist
          shout /censor [on|off]

The shout command echoes a message to the entire mud, prepended by
"Name shouts: ".  It works much the same way as 'say', but echoes to
everyone instead of just to those in your room.

The shout command is often used as a replacement for 'channel', because
it has the added bonus of everyone being able to hear what you say,
regardless of whether they want to or not.
    
This is understandably abused quite often, so the options -d, -a, and -l
were added, with the following uses:

        -d &lt;name&gt;     Denies &lt;name&gt; from shouting.  When they
                      attempt to shout in the future, they will
                      get a denied message.
        -a &lt;name&gt;     allows &lt;name&gt; to shout again.
        -l            Lists everyone who is currently shoutbanned.

Then, history was added to the shout channel, in the form of /last, and
/hist.  /hist backlogs the last 20 or so shouts (depending on your
screen size), and /last lists the last shout made, or the last number of
shouts if a number is passed (ie, shout /last 12.)

The /censor flag can be used to check whether the shout object is
currently censored, and, if you hold Arch rank or above, can be used to
change the censorship status for this command.

NOTES
-----

* Frobs may never shout.
* Mortals cannot generally shout, but there are a few notable exceptions
  that won't be explained here.
* Wizards may shout, but only if they are not shout banned.
* Arches and above may always shout, regardless.
* Only Arches and above may deny or allow shouters.
* All users may list the shoutbanned, and all users may use the
  /last and /hist options.
* It is recommended that you use the channel command as an
  alternative to shouting.
* Mortals that really want to shout can occasionally do so with
  the suicide command.

BUGS

    The -a option doesn't appear to work for everyone.
    
SEE ALSO

    channel, say, tell, whisper, suicide
