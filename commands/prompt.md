---
wikiWrapper: TextArticle
---
Command : Prompt
 
  Syntax
    prompt
    prompt &lt;prompt_string&gt;
    prompt &lt;format_string&gt;
    prompt &lt;id&gt;
 
  Description
    Typing prompt alone will restore your prompt to the last prompt you 
    had set, or ``&gt; '' if no previous prompt was set.
    
    prompt &lt;prompt_string&gt; will set your prompt to prompt_string.
 
    If you are a wizard, prompt &lt;id&gt; will set your prompt to the value 
    of the environment variable "id_prompt"
  
    The prompt formats expand as follows:
      %%          The % character.
      %0          Null.  Evaluates to "".
      %A          Maximum hit points.
      %a          Current hit points.
      %B          Maximum fatigue.
      %b          Current fatigue.
      %C[&lt;Cstr&gt;]  If you are unable to attack, &lt;Cstr&gt; will be sent.
      %C          Same as %C[(NoAttack) ].
      %c[color]   screen color will be changed to color.  Available 
                  colors are:
                  black  red  green  yellow  blue  purple  cyan  white
                  hblack hred hgreen hyellow hblue hpurple hcyan hwhite
                  bblack bred bgreen byellow bblue bpurple bcyan bwhite
                  beep   bold flash  blink   norm
      %D[xxx]     The ASCII character with decimal value xxx.
      %G[&lt;Gstr&gt;]  If you are a member of a group, &lt;Gstr&gt; will be sent.
      %G          Same as %G[(grouped) ].
      %g[&lt;gstr&gt;]  If you are a ghost, &lt;gstr&gt; will be sent.
      %g          Same as %g[(ghost) ].
      %H          The current command number.
      %I[&lt;Istr&gt;]  If you are incapacitated, &lt;Istr&gt; will be sent.
      %I          Same as %I[(incap) ].
      %J          Last command entered.
      %K          Maximum mana.
      %k          Current mana.
      %M[&lt;mstr&gt;]  If you have new mail, &lt;mstr&gt; will be sent.
      %M          Same as %M[(Mail) ].
      %N[&lt;nstr&gt;]  If there are unread posts, &lt;nstr&gt; will be sent.
      %N          Same as %N[(News) ].
      %n          a newline.
      %O[&lt;Ostr&gt;]  If you are following someone, &lt;Ostr&gt; will be sent.
      %O          Same as %O[(following) ].
      %o[&lt;ostr&gt;]  If you are being followed, &lt;ostr&gt; will be sent.
      %o          Same as %o[(followed) ].
      %Q          Total money holdings.
      %q          Your current money holdings.
      %R[&lt;Rstr&gt;]  If you are resting, &lt;Rstr&gt; will be sent.
      %R          Same as %R[(resting) ].          
      %r          The short description of your current environment.
      %S          Your ip name.
      %s          Your ip number.
      %T[&lt;tfmt&gt;]  The current time as returned by strftime(tfmt, time)
                  where time is the current time plus your time_zone 
                  offset hours.
      %T          Same as %T[%C].
      %V          Your evaluation.
      %W          Your wimpy chance.
      %w          Your current mode.
      %X          Your experience.
      %Y          Your current alignment title as shown in 'score'.
      %y          Your current alignment based on a -5 to 5 scale:
                  -5 is demonic, 0 is neutral, 5 is angelic.
      %Z[&lt;Zstr&gt;]  If you are stealthed, &lt;Zstr&gt; will be sent.
      %Z          Same as %Z[(stealthed) ].
 
    If you are a wizard, the following formats also expand:
      %E          The evaluation cost of the last command.
      %e          Remaining evaluation cost after last command.
      %f[&lt;fstr&gt;]  If setv no_finger is on, &lt;fstr&gt; will be sent.
      %f          Same as %f[(nf) ]      
      %i[&lt;istr&gt;]  If setv invisible is on, &lt;istr&gt; will be sent.
      %i          Same as %i[(I) ]
      %L          Your current su'd level.
      %l          Your current real level.
      %P          Your compressed present working directory.
      %p          Your present working directory.
      %U          Your uid.
      %u          Your euid.
      %v[&lt;evar&gt;]  Value of the environment variable &lt;evar&gt;.  "" otherwise.
 
Examples
    Here are some sample prompts:
 
    prompt %c[cyan]%P%c[norm]&gt; would give a prompt looking something like
    this: 
      ~iffy&gt; 
    where ~iffy is the color cyan.
 
    setv debug_prompt 'Last command: %J%nEval Cost: %E%n&gt; '
    prompt debug would give a prompt looking something like this:
      Last command: look
      Eval Cost: 670
      &gt;
    
    prompt HP: %a/%A   Mana: %k/%K   Fatigue: %b/%B   Exp: %X&gt;
    would look something like this:
    HP: 500/500   Mana: 500/500   Fatigue: 500/500   Exp:  206&gt;
