#How to Stop Tracking and Ignore Changes to a File with Git

You run `git status` and there are files Git says are changes but you don't want Git to track those file anymore.  

Here is how you get Git to forget them:

    git update-index --assume-unchanged [path]

An example might be upload files that you uploaded during testing but are not part of your application; somehow you accidentally added them to the Git _"index" (which is the staging area for Git.)_

P.S. I wish Git just had a simple `forget` command!

##References:

- [Stop tracking and ignore changes to a file in Git](http://stackoverflow.com/questions/936249/stop-tracking-and-ignore-changes-to-a-file-in-git)
- [How to Tell Git to Treat a File as Unmodified](0180-how-to-tell-git-to-treat-a-file-as-unmodified.md)

