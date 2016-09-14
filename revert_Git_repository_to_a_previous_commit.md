#Revert Git repository to a previous commit

```` javascript
git log
````

Gets the following output:

````
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

```

##Temporarily switch to a different commit

If you want to temporarily go back to it, fool around, then come back to where you are, all you have to do is check out the desired commit:

````
# This will detach your HEAD, that is, leave you with no branch checked out:
git checkout 0d1d7fc32
````

Or if you want to make commits while you're there, go ahead and make a new branch while you're at it:

````
git checkout -b old-state 0d1d7fc32
````

To go back to where you were, just check out the branch you were on again. (If you've made changes, as always when switching branches, you'll have to deal with them as appropriate. You could reset to throw them away; you could stash, checkout, stash pop to take them with you; you could commit them to a branch there if you want a branch there.)

