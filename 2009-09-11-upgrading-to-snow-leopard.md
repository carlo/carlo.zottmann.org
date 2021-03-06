Title: Upgrading to Snow Leopard
Date: 2009-09-11 15:19:18
Slug: 2009/09/11/upgrading-to-snow-leopard
Tags: apple, en, microsoft, snow leopard


I've made the switch from Leopard to Snow Leopard today. First, I took the
necessary steps, of course: checking [this handy app compatibility list][1],
running [AppFresh][2], then [SuperDuper!][3]. While the overall install went
smoothly on my mid-2009 iMac 24", I ran into some issues which I'd like to jot
down real quick.

  * Terminal.app has issues with my favourite programming font, [Inconsolata][4]. The font isn't rendered at all, which is a pain. I went with Menlo (the new monospaced font coming with Snopard) for the time being. (In Textmate, Inconsolata renders just fine.)
  * The _Language & Text_ preference pane refuses to allow me to use the "German - Microsoft" layout. It's a 32-bit vs 64-bit issue with [MS' Intellitype software][5] (which is needed for my Natural Ergonomic Keyboard 4000) — the 32-bit drivers can't be used in 64-bit apps, and the keyboard reverts to its default "German" layout. According to [this Apple support board post][6] it's not even clear whether there'll be a 64-bit Intellitype software at some point. Saying this is inconvenient would be an understatement.
  * I've switched from 1Password 2 to [1Password 3 Beta][7] since 1Password 2 would've required me to run Safari in 32-bit mode; v3 doesn't. Looking good. Can't say more due to the NDA. :)

The rest seems to be fine. Standing out most:

  * Booting the iMac seems to be faster now.
  * Image Capture finally recognizes my CanoScan LiDE 200 scanner out of the box! (About time.)

All in all, not a bad update. The family license goes for €49, so I didn't
have to think long about it.

**Update:** I was able to fix the keyboard problem! Today I found [Ukulele][8], an Unicode keyboard layout editor. After downloading it, I've poked around the DMG and found two files, `LogitechGerman.keylayout` and `LogitechGerman.icns`. After copying them to the `/Library/Keyboard Layouts/`, all that was left was opening the _Language & Text_ preference pane and activating the "Logitech German" layout. Dynomite!

   [1]: http://snowleopard.wikidot.com/?utm_source=MailingList&utm_medium=email&utm_campaign=Mailplane+and+Snow+Leopard
   [2]: http://metaquark.de/appfresh/
   [3]: http://www.shirt-pocket.com/SuperDuper/SuperDuperDescription.html
   [4]: http://www.levien.com/type/myfonts/inconsolata.html
   [5]: http://www.macupdate.com/info.php/id/29220/microsoft-intellitype
   [6]: http://discussions.apple.com/message.jspa?messageID=10124424#10124424
   [7]: http://www.switchersblog.com/2009/08/update-1password-on-snow-leopard.html
   [8]: http://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&item_id=ukelele
