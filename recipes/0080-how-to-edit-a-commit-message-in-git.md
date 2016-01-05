#How to Edit a Commit Message in Git

To edit the message for your most recent commit:

    git commit --amend -m "{New commit message}"
    
To edit a message from more than a few commits back _(either of these work):_

    git rebase --interactive {parent_of_flawed_commit}
    git rebase -i {parent_of_flawed_commit}
    
When the editor pops up change `pick` to `reword` and reword your commit message, then save the file and Git will do its magic.

Then to push to your remote, if needed _(either of these work):_

    git push {remote} {branch} --force
    git push {remote} {branch} -f

Often you'll be using `origin` and `master`, for example:

    git push origin master --force
    git push origin master -f

##References

- [Edit an incorrect commit message in Git](http://stackoverflow.com/questions/179123/edit-an-incorrect-commit-message-in-git)    
