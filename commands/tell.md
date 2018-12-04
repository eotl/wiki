---
wikiWrapper: TextArticle
---
Command: Tell.
Format:  tell &lt;player&gt; &lt;message&gt;
Example: tell zippo wah, the mud is broke!
 
     The tell command is used to send a message across the mud to
other players currently on the mud or to people on other muds.  Valid
syntax follows:
 
tell &lt;what&gt; &lt;message&gt;
  This will send the message to the specified person/people.
  What can be any of the following:
 
  -&lt;category&gt; sends a tell to everyone in &lt;category&gt; if it is one of
       your notification categories.
 
  :&lt;rclist&gt; tells to everyone on the specified rclist. Go into the
       mailer and type 'list' to get a list of the rclists.
 
  . tells to whoever you last sent a tell to. This can be one person
       or a group of people.
 
  &lt;person&gt; send a tell to person.
 
  &lt;person&gt;@&lt;mud&gt; send an intermud tell to person at mud.
 
  
  Any one or combination of these can be used.  When more than one
  group is selected, a comma ',' must be used to seperate them.
 
  Example:                                    
      tell bob, ., :eternal, -friends hi
   
      This would tell bob, the group you last sent a tell to,
      everyone in the eternal cabal and everyone in your friends
      notification list.
 
  It is not necessary to have a space after each comma.
  All exclaimation marks and spaces will be ignored if in the &lt;what&gt;
  section of the tell.
  Capitalization is ignored in the &lt;what&gt; portion of the tell. "BOB"
  is the same as "bob".
     
 
tell /last (num)
  This will display the last tell you recieved. The optional argument
  will display the last num tells up to the max of 20.  This setting
  is saved.  Example: If you did tell /last 10, the next time you did
  tell /last it would display the last 10 tells.

tell /last (name)
  This will show you all the tells in your history that came from
  name.

tell /last (regexp)
  This will do a regexp search through your last 20 tells for regexp.
 
tell /hist 
  This will display the last 20 tells.
  
-Tyrus


See also: reply, say, whisper.
