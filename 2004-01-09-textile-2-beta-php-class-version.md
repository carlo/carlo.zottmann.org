Title: Textile 2 beta - PHP class version
Date: 2004-01-09 05:01:17
Slug: 2004/01/09/textile-2-beta-php-class-version
Tags: code, en, hacking, php


I've been toying around with Dean Allen's mui funky [Textile][1] for a while
by now, and finally, as I'm approaching a certain state of development in
G-Blog.net v2, I think I have a use for it. It'll most likely be the
formatting gizmo of choice for the next version of this very site.

Anyways, while the original [version 2.0 beta][2] is great, it's somewhat
annoying to have as part of an object-oriented framework, since this version
is basically just a number of functions. The code is good, but the frame
that's holding it isn't. So I've took the liberty of refactoring (kind of) the
code into a PHP class which can easily be used in an OO context. I didn't add
to its original feature set, I've merely restructured the whole thing a bit.

How to use it:


    * Example: get XHTML from a given Textile-markup string ($givenstring)
    *
    *        $textile =& new Textile();
    *        print $textile->TextileThis($givenstring);
    *
    * Example: get Textile-markup from a given XHTML string ($givenstring)
    * Please note: This method is still work in progress.
    *
    *        $textile =& new Textile();
    *        print $textile->DeTextileThis($givenstring);


So, without further ado: [On to the Textile 2.0 beta class version!][3]

   [1]: http://www.textism.com/tools/textile/
   [2]: http://www.textism.com/article/739/
   [3]: http://docs.g-blog.net/code/Textile/2.0beta_class_version/class.textile.php.txt
