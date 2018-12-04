---
wikiWrapper: TextArticle
---
Command : Bid.
Format  : bid &lt;amount&gt; on &lt;lot number&gt;, bid &lt;lot number&gt;, bid
Example : bid 100 on 3, bid 3, bid

      This command has three different uses.

      First use is how you actually bid on an item that has been auctioned.
You must bid at least 10% or 100 coins (whichever is more) higher than the
previous bid.  You may also use "min" instead of an amount to bid the minimum
required amount.  Each bid will add 30 seconds to the remaining duration of
the auction.  If you are outbid you will be told.  If you are the seller you
are informed of each bid.  Once you bid, the money is taken directly from
your account at that time.  If you are outbid your money is put back.

      Second use will give you some stats on that lot.  The current amount
bid, the time remaining, the short desc, the long desc, any contents.

      Third use shows everything currently on the auction block.

      When there are around 30 seconds left in an auction the auctioneer will
announce going once on auction channel with the item desc and the current bid
amount.  When there are approximately 15 seconds left he will announce going
twice.  He will then announce the results of the auction.  These messages all
use the auction channel color.  Messages sent directly to you by the auction
house can be colored via the color command.

See also: auction, color
