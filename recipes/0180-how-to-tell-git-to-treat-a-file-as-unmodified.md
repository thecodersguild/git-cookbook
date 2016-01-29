#How to Tell Git to Treat a File as Unmodified

You have a file that has changed, but for _right now_ you want Git to ignore that the file has changed when you run `git add .` or `git commit -a`. 

So use this command: 

    git update-index --assume-unchanged {filename}
    
Assuming a file named `'MyFile.txt'`:

    git update-index --assume-unchanged MyFile.txt
    
Then you can run the following without committing `MyFile.txt`:

	git add .
	git commit -m "Your commit message here"
	
After you are finished ignoring `MyFile.txt` you can run:

	git update-index --no-assume-unchanged MyFile.txt
    
##References

- [temporarily ignoring files](http://gitready.com/intermediate/2009/02/18/temporarily-ignoring-files.html)    
- [How to Stop Tracking and Ignore Changes to a File with Git](0150-how-to-stop-tracking-and-ignore-changes-to-a-file-with-git.md)
