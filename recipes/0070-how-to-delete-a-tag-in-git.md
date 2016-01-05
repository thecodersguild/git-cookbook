#How to Delete a Tag in Git

You have tagged a commit and realize that you need to undo it. Maybe you need to sneak in one more commit before the tag?

To delete a Tag in Git:

    git tag -d {my_tag}
    
So, for example:

    git tag -d 2.7.3
    
##Removing a Tag from your Git Remote
If you have already pushed that tag to your remote, then **any of these** will remove it from the remote:

    git push origin :refs/tags/{my_tag}
    git push origin :{my_tag}
    git push --delete origin {my_tag}
    
Following the above example that used tag `2.7.3`:

    git push origin :refs/tags/2.7.3
    git push origin :2.7.3
    git push --delete origin 2.7.3
    

##References

- [How to: Delete a remote Git tag](https://nathanhoad.net/how-to-delete-a-remote-git-tag)
- [How do I remove or delete a tag from a Git repo?](https://confluence.atlassian.com/bitbucket/how-do-i-remove-or-delete-a-tag-from-a-git-repo-282175551.html)
- [How to delete a remote tag?](http://stackoverflow.com/a/5480292/102699)
- [Remove a Git Tag From Github When There is **Also a Branch of the Same Name**](http://blogs.perl.org/users/mr_muskrat/2010/10/remove-a-git-tag-from-github-when-there-is-also-a-branch-of-the-same-name.html)
- [Adding and Removing Tags on GitHub](http://wptheming.com/2011/04/add-remove-github-tags/)    
