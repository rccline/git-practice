# git-practice
A Repo for practicing Git

### Undo changes in git ^[Peter Tichy's amazing YouTube channel: *ihatetomatoes* (*https://www.youtube.com/watch?v=MIFQwHlEI9o&t=324s*)]  

* **reset**  
1. stage - unstage  
2. track to untrack  
3. *reset* a previous commit  
4. reset a specific file to previous commit  
5. Get specific chages from specific commit  

* *git log*  
  - (HEAD -> master)  *the local commits*    
  - (origin/master, origin/head)  *commmits in the repo*  
  
* **How to unstage**  
  - *git diff --cached*  
  - *git diff --name-only --cached*  
  - *git reset <filename>*  
  
* **Unstage all changes**  
  - git add *.* 
  - *git reset HEAD*  
  
* **How to trash changes**  
  - *reset* empties the staged files 
  - files in working direcdtory are left alone.  
  - *git reset*  or *get reset <filename>*  
  
* **Remove the file completely**  
  - *git reset --hard* 
  
* **replace the file in working directory with the staged file**:  
  - *git checkout <filename>* 
  
### git log -'-pretty=oneline  

When you run git log with the --pretty=oneline option, it displays each commit on a single line, along with a few key pieces of information about each commit. In the output you provided, the six pieces of information displayed for each commit are:

* *Commit hash*: 9fbbad0ff497822aa41b7a77abea959e8f124e8c is the unique identifier for the commit. It is a 40-character string generated from the contents of the commit.

* *(HEAD -> master, origin/master, origin/HEAD)*: This indicates *the current branch* and *the remote branches* tracking it. **HEAD** refers to the current branch, and **master** is the name of the local branch. origin/master and origin/HEAD are the names of the remote branches that are tracking the local master branch.

* *Commit message*: Add Undo changes in git is the summary of the changes made in the commit. This message is usually written in the present tense and should provide a clear and concise description of the changes made.

The format of the output from git log --pretty=oneline can be customized by using other --pretty options, or by using a custom format specified with the --format option.
