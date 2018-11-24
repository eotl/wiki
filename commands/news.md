---
wrapper: "../../../js/components/wiki/TextArticle"
---
COMMANDS:

  -p              -- Go to first page with unread articles.
  -p #            -- Go to page number #.
  -p <expression> -- Go to page containing <expression> or, if there is more
                     than one, list all pages containing <expression>.
  -p list         -- List all pages that you are subscribed to.
  -p list new     -- List all pages you subscribe to that have new articles.
  -p list all     -- List all possible pages to subscribe to.

  -h              -- Show the headlines of unread articles on current page.
  -h #            -- Show all headlines from 1 to # on current page.
  -h old          -- Show all headlines on current page.

  -r              -- Begin reading all new articles on current page.
  -r #            -- Read article number # on current page.
  -r #,#, .. #    -- Read all those article you specify on current page.

  -w              -- Write an article ON CURRENT PAGE.
  -w title        -- Write an article ON CURRENT PAGE with title 'title'.
  <SPOILER>       -- Insert spoiler space into an article.  This only applies 
                     the first time it appears in an article.  The <SPOILER> 
                     tag on a line by itself will make sure that there is 
                     more than a full screen of blank space in your message, 
                     so those who don't want to read spoilers can exit from 
                     the message.

  -e #            -- ERASE ARTICLE NUMBER # ON CURRENT PAGE.

  -m #            -- Mark all articles as read up to number # on current page.
  -m SUB          -- Mark all subscribed pages as read.
  -m SUB #        -- Mark all subscribed pages as read to article #.
  -m ALL          -- Mark all articles on all pages as read.
  -m ALL #        -- Mark all pages as read up through article #.

  -s #            -- Subscribe to page number # (on the ']p list all' list).
  -s all          -- Subscribe to all possible pages.

  -c #            -- Cancel subscription to page number # (']p list' list).
  -c !            -- Cancel current news page.
  -c all          -- Cancel all subscriptions (?!).

  -b <player>     -- Read last post by <player> already read on current page.
  -b <player> all -- Read all posts by <player> on current page.
  -b <player> #   -- Read all posts by <player> from number # on current page.

  -x # file       -- Xerox article number # on current page to ~/file. (Frob+)

  -create Title   -- Create 'The Title Page' (Arch+, duh).
  -hose Title     -- Hose 'The Title Page' (Arch+, duh).
  -mod Title      -- Modify settings for 'The Title Page' (Arch+, duh).
  -move Title #   -- Move 'The Title Page' in the list (Arch+, duh).
  -stat           -- List the settings for your current page (Frob+).
  -stat Title     -- List the settings for 'The Titled Page' page (Frob+).
  -stat all       -- List the settings for all news pages (Frob+).

NOTE:

  In all cases where the `-' character is used, you could also use `]' or
  `news '.  This is so that all keyboard types are supported.
