Title: Twitter Twerp Scan
Date: 2008-04-28 08:22:09
Slug: 2008/04/28/twitter-twerp-scan
Tags: en, hacking, javascript, twerp scan, twitter, yahoo! pipes, yui libraries


Over the last few days I’ve pursued my idea to build a “Twitter spammer
detector” of sorts using only client-side technologies. I didn’t feel like
setting up server components at all.

What was it supposed to do? It should check the number of followers of
everyone on your contact list, the number of people they are following, and
the ratio between those. If the person is following more than 1000 people (can
be customised), and has a Following-to-Followers ratio higher than 1:1 (can be
customised), you’d be informed (by a handy “Block” link).

Thanks to [Pipes][1], the [YUI libraries][2] and the [Twitter][3] API
returning JSON, I was able to finish the first version of [Twitter Twerp
Scan][4] in a relatively short period of time.

My Javascript-fu is still a bit weak, but getting better. It’s a nice change
to only have one local file to work with (excluding CSS, of course).

Over the weekend, the traffic to that page increased quite a bit, mostly
because [several][5] [people][6] liked the idea enough to link the site.

I've set up a Twitter account for service updates etc. -- [twerpscan][7]. The
rest of my tweets will go to [Carlo][8] as usual.

   [1]: http://pipes.yahoo.com/
   [2]: http://developer.yahoo.com/yui/
   [3]: http://twitter.com/
   [4]: http://twerpscan.com/
   [5]: http://www.downloadsquad.com/2008/04/27/twitter-twerp-scan-block-twitter-spammers/
   [6]: http://twitter.com/leolaporte
   [7]: http://twitter.com/twerpscan
   [8]: http://twitter.com/Carlo
