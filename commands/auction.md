---
wrapper: "../../../js/components/wiki/TextArticle"
---
Command : Auction.
Format  : auction &lt;item&gt; for &lt;amount&gt; coins, auction status, auction &lt;text&gt;
Example : auction sword for 100 coins

      This command has three different uses.

      First use is to put something up on the auction block.  Once an item is
put up for auction it is transferred to a secure location to protect the
investment of the auction house.  An auction starts at 30 minutes displayed as
1800 seconds.  Once someone has bid it will drop to 3 minutes to go, displayed
as 180 seconds.  See bidding for more on the actual guts of how the auction
runs once started.  Once it is over the money, minus a 5% handling fee, is
transferred to the buyer's bank account from the seller's and the item is
transferred to the buyer's inventory.  
      When you first put the item up for auction you will be asked if you wish
to buy the item back if no one bids on it.  The buyback fee is the lower of
the starting bid amount or 500 coins.  If no one bids on the item and you do
not select buyback then the item is kept by the auction house.

      Second use will tell you if you have anything on the block and what
the current status (who's bid, how much, time left) of the auction is.

      Third use is to talk on the auction channel.  This is essentially an
alias for 'channel auction'.

      Messages relating to the auction are sent to the seller, bidders, and
on the auction channel.  This is covered more in depth in the bid file.  The
messages can be colored, see the color command.

      It is worth noting that once you put an item up for bid you do not need
to remain logged on for the auction to proceed normally.  Any money you make
from items put up for bid is put directly into your account regardless of
you being logged in or not.

See also: bid, color
