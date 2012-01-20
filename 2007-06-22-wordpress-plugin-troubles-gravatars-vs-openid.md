Title: Wordpress plugin troubles: Gravatars vs. OpenID
Date: 2007-06-22 20:28:57
Slug: 2007/06/22/wordpress-plugin-troubles-gravatars-vs-openid
Tags: code, en, hacking, openid, wordpress


So [Robert notified me][1] that his [Gravatar][2] didn’t show up in my
comments. After some debugging I found and fixed the problem.

The [Gravatars plugin][3] works fine with the default comments, but not with
the [wpopenid / WP-OpenID+ plugin][4]. Son of a Perl script!

Turns out in the gravatars2.php only checks for the known comment types:
_comment_, comment_type _trackback_, comment_type _pingback_. Comments made
using an OpenID account (on Wordpress installs with the aforementioned OpenID
plugins enabled) are saved with comment_type _openid_. Aha!

So here’s the fix: in gravatars2.php (you know where to look for it), search
for

bc. if ((’’ $comment->comment_type) || (‘comment’ $comment->comment_type)) {

and replace it with

bc. if ((’’ $comment->comment_type) || (‘comment’ $comment->comment_type) ||
(‘openid’ == $comment->comment_type)) {

There are two occurences. (The line breaks are usually not there, it’s all on
one line.) Change, save, and that’s it.

Tip to the hat goes to [Robert][5] for pointing out the bug, and narrowing it
down. Appreciated! :)

   [1]: http://carlo.zottmann.org/2007/06/21/weissbier-with-timberlake/#comment-7418
   [2]: http://site.gravatar.com/
   [3]: http://zenpax.com/gravatars2/
   [4]: http://wordpress.org/extend/plugins/openid/
   [5]: http://blog.hooloovoo.net/