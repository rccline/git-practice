### Revert  
* Allows us to remove a single commit  
* This is why you want your commits to be *atomic*  
  - if you commit numerous files at once, a Revert will take out all of those files.  

* add a text file.  Add one line, commit
* add second line, commit  
* then revert the second line.  

### To avoid conflict  
* Go to the file you want to change.
* git checkout #hash
* make change  
* git revert #hash  
 

### Revert CONFLICT  
In rstudio, using git bash, I ran git revert 317a9c4 and I got this message:  CONFLICT (content): Merge conflict in revert-1.txt.  Could ot revert 317a9c4... Add revert-1.txt with 'line 1.'   How do I resolve the content and revert 317a9c4?  

To resolve the conflict, you need to edit the revert-1.txt file in Rstudio.

1. Open the revert-1.txt file in Rstudio.
You will see the conflicting changes marked in the file.

2. Edit the file to resolve the conflict by choosing the appropriate changes that you want to keep.
3. Save the file.
4. Run the command git add revert-1.txt to stage the changes in the file.
5. Run the command git revert --continue to complete the revert process.
6. Verify that the conflict has been resolved by running git status.

You should now be able to successfully revert the 317a9c4 commit. 

### [Eddie Jaoude's method to **git revert**](https://www.youtube.com/watch?v=YUHS5Ana7Jw) 

* git status -s  
* git whatchanged  
* git diff master  
* git checkout master -- package-lock.json  
* git status -s  
* git commit -m "fix package lock file" . 
* git status -s  
* git diff master  
  - will only see the changes to that one file  
  



