Title: 0Spam.com review
Date: 2004-01-03 16:43:25
Slug: 2004/01/03/0spam-com-review


After being annoyed with spam emails for quite some time now (who isn't?), I
was setting up some perimeter defenses to keep the viagra and penis
enlargement offers out of my eyesight. [SpamAssassin][1] on my server (its
threshold is set pretty high after it accidently filtered out some good
mails); [Firebird][2]'s spam filters are working for me at home, and the
[SpamBayes Outlook Plugin][3] is keeping me sane in the office. (Well, at
least when it comes to email.)

But is it enough? The good the filters are, I still am overwhelmed by spam
when I open up my webmail interface -- the mail in there is already filtered
by SpamAssassin but not yet processed by my client filters.

Or am I? A couple of weeks ago I've discovered [0Spam.com][4], a relatively
new kid on the block. 0Spam's concept is a tad bit different from the usual
spam filters, since it's making use of whitelists and blacklists. Here's how
it works.

Every ten minutes or so, the 0Spam gizmos check my POP3 account. If they find
mails from senders which are not on my whitelist yet, they're are moved to the
0Spam server, and the sender is sent a validation mail. Now the sender
(assuming it's a real person and not a viagra-powered penis enlargement robot)
has a week to visit the link in the mail where s/he is presented with a
validation code s/he has to enter manually. Once this is done, the 0Spam
gizmos know the original mail came from an actual human, and the particular
mail is moved from the 0Spam server back to my POP3 account. The sender is
then marked as "good" for future reference, which means that once you've
visited that validation link after mailing me, you won't have to do it ever
again. You're validated once, and that's enough.

There are a number of settings I can edit in my account. First of all, I can
set the time span the sender is given to validation link - options range
between 1 to 14 days. If the sender doesn't visit the validation page within
that time frame, the mail will be discarded. Second, I can set up more than
just one POP3/Hotmail/Yahoo account to be checked periodically by ospam.
Third, I can influence the auto-whitelisting behaviour (the above mentioned
behaviour of automatically marking a validated sender as "good" for the
future).

Entering whitelists and blacklists.

A so-called "whitelist" is a list of good senders, people or domains that are
trusted. The email whitelist is a list of all email addresses that are allowed
to send you mail, which is kept up to date automatically. However, you can
import your address book into the email whitelist to make it easier for your
contacts to verify their first email to you. The domain whitelist allows you
to whitelist any message from one or more specified domains and the keyword
whitelist lets any mail into your inbox that contains any word or phrase you
provide. Just to make sure I don't miss any important mails by people or sites
I know, I've imported my address book, and fed a number of domain name
fragments to the domain whitelist, for instance "amazon", "bloglines.com",
"bungie", "dreamhost.com" and "ebay". As you can see, you don't have to
provide full domains; allowing "amazon" to mail me means mails from amazon.de,
amazon.com, amazon.ca etc. go thru. You get the picture.

Blacklists are the exact opposite, but they have to be treated more carefully.
You may configure 0Spam.com to block mail from your account if a message is
from any address in the email blocklist or if it contains a word or phrase
found in the keyword blocklist. It's not recommended to use the email
blocklist to block spammers, as most spammers use email addresses that change
each time they send out mail. Sometimes it _is_ nice to have a blocklist, tho.
For instance, after receiving 20 "security patches" from "Microsoft Support" a
day (I'm talking about the Blaster worm which was sending itself across the
net using supportATmicrosoftDOTcom as fake sender), I've put the said mail
address on the blocklist, and the mails were discarded as soon as 0Spam
discovered them.

So far, the service works like a charm for me. The key to leading a care-free
life with 0Spam without loosing all your friends is to import your address
book and to think hard about what domains should be whitelisted. Remember -
even Amazon and Ebay are using bots to send out different types of valid
mails, and these bots will not make it thru the validation. Therefore you
should definitely whitelist these domains you know for certain you'll be
receiving good mails from. I highly recommend skimming thru your mail client's
trash folder to see which sites are "rightfully" mailing you periodically.

The great thing about 0Spam is that it works with almost every email account
on the planet. And you don't even have to change anything in your mail client
setup, because it's not really sitting between you and your mailbox, it's more
like an automated watchdog doing its rounds roughly every ten minutes,
grabbing everything from your mailbox that doesn't seem to belong there.

By the way, if your mail client is always open and getting new mails from the
server every minute or so, 0Spam will not work, because the mail client will
most likely grab the mails before 0Spam can. Hence, the filtering will fail.
So it's recommended to make your mail client check for new messages every 30
minutes or once per hour. This might seem long, but remember, you're not
getting that much "good" mails anyways -- you're just not noticing it because
of all the spam. ;)

Also, once 0Spam took a peek at a mail, it'll be marked as read. I'm not sure
whether or not this applies to Hotmail accounts as well, but it does for my
plain old vanilla POP3 account. The mails are marked as unread in my mail
client after downloading them from the server, tho, so I don't think that's a
problem. It sure is not for me.

Alltogether I'm very happy with 0Spam. It's doing a fine job. The service is
running quite stable so far, even tho it's still in development. And even if a
spam mail is making it thru the 0Spam filter because it's claiming to be from
buyviagragoddammitATebayDOTcom - my Firebird will catch it client-side.

So, if you're still having problems with unsolicited emails, give [0Spam][5] a
whirl. The site is a bit plain, but the service is free and working. I can't
tell you whether there are hidden drawbacks or not. Theoretically speaking,
there is a chance someone else's filter will mark the 0Spam validation mails
as spam. I'm not aware of such a case, but you'll never know. Also, some might
argue that this type of service (whitelisters) are "against" the "open
character" of email, i.e. the idea behind the medium - everyone can be reached
by everyone else. I say the medium went downhill once email marketing took
off. Personally, I'm rather talking to others using Jabber/ICQ/AIM than email;
it's a more fluid conversation. YMMV.

Well, that's it. From the "spam fuckers made our live worse" front, this is ye
olde Gossip.

   [1]: http://www.spamassassin.org
   [2]: http://www.mozilla.org/projects/firebird/
   [3]: http://spambayes.sourceforge.net/windows.html
   [4]: http://www.0Spam.com
   [5]: http://www.0spam.com
