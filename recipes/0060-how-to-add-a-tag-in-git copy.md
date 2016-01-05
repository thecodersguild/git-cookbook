#How to Add a Tag in Git

You have a commit that you want to associate a name with so you want to _"tag"_ it.

To add a Tag in Git:

    git tag -a {my_tag} -m "{My Message}"
    
So, for example:

    git tag -a 2.7.3 -m "Version 2.7.3"
    
##Pushing Tags to  your Git Remote

To push you tags to your remote:

    git push --tags    
    

##References

- [Git Basics - Tagging](http://git-scm.com/book/en/v2/Git-Basics-Tagging)
- [Adding and Removing Tags on GitHub](http://wptheming.com/2011/04/add-remove-github-tags/)    
