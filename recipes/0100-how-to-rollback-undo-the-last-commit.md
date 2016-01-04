#How to Rollback/Undo the Last Commit

You just made a Git commit you realize was a mistake and you want to roll it back and **for everything to be as if you never made the commit.**  Easy:

    git reset --soft HEAD~

Why would you need this?  Maybe you committed too many files and/or changes.  Maybe you had a typo in the commit message.  Maybe you realized you committed a bug. You don't want to throw away anything, you just want a do-pver. You want everything back like it was the instant before you made the mistaken commit.  

So **reverse time with this technique**, sadly there are few other things in life that are as easy to reverse.

For more explanation on this see [this answer](http://stackoverflow.com/a/927386/102699) on StackOverflow. 


###Warning:
If you have **pushed** since your commit, you really should not do this unless you are the only one commiting to your remote repo because this rollback erases history.  Caveat emptor!



     
