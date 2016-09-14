#Revert Git repository to a previous commit

´´´´ javascript
git log
´´´´

Gets the following output:

$ git log
commit a867b4af366350be2e7c21b8de9cc6504678a61b`
Author: Me <me@me.com>
Date:   Thu Nov 4 18:59:41 2010 -0400

blah blah blah...

commit 25eee4caef46ae64aa08e8ab3f988bc917ee1ce4
Author: Me <me@me.com>
Date:   Thu Nov 4 05:13:39 2010 -0400

more blah blah blah...

commit 0766c053c0ea2035e90f504928f8df3c9363b8bd
Author: Me <me@me.com>
Date:   Thu Nov 4 00:55:06 2010 -0400

And yet more blah blah...

commit 0d1d7fc32e5a947fbd92ee598033d85bfc445a50
Author: Me <me@me.com>
Date:   Wed Nov 3 23:56:08 2010 -0400

Yep, more blah blah.