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
  - *git acheckout <filename> 
