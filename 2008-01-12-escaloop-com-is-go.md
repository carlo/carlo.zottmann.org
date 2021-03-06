Title: escaloop.com is go!
Date: 2008-01-12 14:44:34
Slug: 2008/01/12/escaloop-com-is-go
Tags: announcements, en, escaloop, hacking, ramaze, ruby, yahoo! pipes


A few months ago I was talking to [Hendrik][1] about lifestreams, and in my
ongoing struggle for his undying love (as a friend), I’ve whipped up a little
somethingsomething using the wonderful [Yahoo! Pipes][2].

_“Lifestream?”_, you ask. _“What the deuce is a lifestream?!”_ A good
question. A lifestream is basically a big bucket where all the updates and
update notifications from your blog, your [ADD-induced][3] Twitter posts, your
Flickr uploads etc come together in one concise way so it’s easier for others
to ignore them. ;) Also, you only have one URL to hand out to hot women (or
men) in pubs because the stream inadvertedly works as a hub page, too!

Now, while the prototype was quickly hacked together, it felt clunky. Sure,
you can pass a dozen URLs or so to the pipe, but what if the URLs would
change? Or if you wanted to add a new one or delete one from the list? Then
it’d be a lot of tinkering with the script call in your HTML code.

So I had the idea to build a site where you could configure the list of URLs
and the layout and everything, and which would give you a HTML badge for your
blog or site, a snippet that wouldn’t change.

[And today, I proudly open **escaloop** to the public.][4]

I feel it’s _good enough_ to test the waters, I believe. I’ve played around
with it, fiddling with different implementations on different types of pages,
and it looks okay. I guess I could try to think of every possibility for every
site on earth, but we know how that would turn out.

It certainly [looks fine on my own blog][5]. (Considering that I don’t have
that many active feeds, that is.)

So with that, I’ll release [escaloop][4] into the wild. It’s still a bit rough
around the edges, and there might be bugs. That said: Please take a look, play
around with it, build yourself a badge or two for your site, blog, MySpace
page, whatever. If you have feedback, [please let me know in the escaloop
Google Group][6].

Have fun, Carlo

PS: You might ask what took me so long. In my defense, I am a lazy bastard.
Also, I wrote the first rough draft in Python, then switched to Ruby. There
I’ve wrote the first prototype using the [Sinatra][7] DSL, and finally settled
to make use of nifty lightweight [Ramaze][8] framework. (By the way, Sinatra
is nice, but not what _I_ was looking for.)

During the last few months I’ve also _had to_ put a lot of time into [Mass
Effect][9], which is a great game. You understand.

   [1]: http://mornography.co.uk/
   [2]: http://pipes.yahoo.com/
   [3]: http://en.wikipedia.org/wiki/Attention-Deficit_Disorder
   [4]: http://escaloop.com/
   [5]: http://carlo.zottmann.org/lifestream/
   [6]: http://groups.google.com/group/escaloop
   [7]: http://sinatra.rubyforge.org/
   [8]: http://ramaze.net/
   [9]: http://masseffect.bioware.com/
