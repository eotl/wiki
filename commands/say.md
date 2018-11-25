---
wrapper: "../../../js/components/wiki/TextArticle"
---
The Say Command

     The say command is used to echo messages to anyone who is the 
room with you.  Valid commands are:

say &lt;what&gt;:
  This will echo the string &lt;what&gt; to the room you are in.
  
' &lt;what&gt;:
  The say command can be abbreviated with a single ' making it easier
  to type.  It works just as though you were typing say.

say /last &lt;number&gt;
  This will display the conversation you've heard. The optional argument
  will display the last number of items up to the max of 20.
  
say /last &lt;name&gt;
  This will show you all the conversationin your history that came from
  name.

say /last &lt;regexp&gt;
  This will do a regexp search through your last 20 history items for 
  regexp.

say /hist
  This will display the last 20 items of conversation.


ALSO SEE: tell, whisper

