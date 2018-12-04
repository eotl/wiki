---
wikiWrapper: TextArticle
---
Command : Color
Format  : color &lt;options&gt;

To set the default colors simply type 'color default'.
To list all colors set type 'color list'.

To set the color that you would like for any of the commands that are
possible to be colored (type 'color' to list these). Type 'color' followed by 
the name of the command, followed by '&lt;opts&gt;' where &lt;opts&gt; can be one or more
of the following:

    off            -- Disable coloring of this command.
    default/norm   -- Sets the coloring for this command to normal.
    default2/norm2 -- Sets the coloring for this command to normal2.
    beep           -- Adds a beep (^G) to this command.
    whole          -- Colors the entire message instead of just the prefix.
    flash/blink    -- Causes this command to flash.
    bold           -- Causes this command to use high intensity colors.
    underline      -- Uses the VT100 code for underlining for this command.
    reverse        -- Uses the VT100 code for reversing fore/backgrounds.
    &lt;fore&gt;         -- Sets the foreground color for this command to &lt;color&gt;.
    &lt;fore&gt;,&lt;back&gt;  -- Sets the foreground color to &lt;fore&gt; and the background
                      color to &lt;back&gt; for this command.

Valid colors for &lt;fore&gt; and &lt;back&gt; are:

    black    red    green    yellow    blue    purple    cyan    white

Some examples:

    Example: color say cyan,black beep
    Example: color tell beep bold yellow
    Example: color shout flash reverse

The order of the options does not matter, except that those you type first
will take precedence over the last ones, although there is no need to use
conflicting options in the same command, bogleg.

The commands tell, say, go, and shout can also have another form of coloring
added to them. This coloring involves adding a color in [] into the argument
of the tell you send.
    eg. tell mortal this color will be [red]red.
Typing [RED] instead of [red] will make the color bold red instead of normal
red. The color will work from anywhere in the tell except as the last thing.
'set extra_color off' to stop others from sending you these extra colors.

See also: hp, ansi
