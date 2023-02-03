# git-practice (Readme2)
A Repo for practicing Git


### Resources:

1. [Eddie Jaoude Part3](https://www.youtube.com/watch?v=LsQjcX3b0ZM&list=PL4lTrYcDuAfxAgSefXftJXbhw0qvjfOFo&index=3)  

2. [Becoming a Data Scientist - Beginner Git#5](https://www.youtube.com/watch?v=UmE0uf5UMzA)

### git commands  

* Create a new branch to do *pull requests*  
* git checkout -b *branch_name*  
* Can do your work in a branch  
  - You can create *pull requests* in a branch to go to master    
  - if you make a mistake, **if you push something up and your history becomes a mess, you can do forced pushes to your branch and rewrite your history *if no one else is working in your branch*  **  

### How do you rewrite history?  
* **git reset**
* **git reset --soft HEAD~1**  
  - the *~1* takes you back one commit; 
  - *~2* takes you back two commits. 
  - soft means **keep changes**  
  - hard means **discard changes**  
* **Be careful with the *reset* command**  
  - *reset* is also used to stage and unstage files  
* **Example-1: Stage and unstage files**  
  - git add README.md  
  - git status -s  
  - git reset README.md
  - git status -s 
  
* **Example-2 (2:28) *Make a mistake and commit everything, not the file you intended***   
  *git commit -m *test commit* .*  
  - git commit -m "test commit" . 
  - BUT, you did not want to commit all the files.  
  - git status -s  
  - **if you *git revert* it will do another commit, with the complete opposite of those changes??  
  So, I would have to remake those changes to the README.md  *and* it would leave the history that you do not want to be there.  
  - git reset --soft HEAD~1 
  - git whatchanged  
  
* **REITERATE**  
  -  git commit -m "test commit" . 
  - git status -s 
  - **git diff --stat origin/master**
  - git reset --soft HEAD~1
  - git whatchanged 
<br> 
<br> 

###  **WHAT I LEARNED**  

* Cannot reset initial commit.  
* TO PUSH the new branch:    
  - 1. Move to new branch on local; then:     
  - 2. **git push -u origin dev1**  
  
### Make Changes to global config alias file.  

* Global config will open in safe mode unless you run the following code first:  
* git config --global --unset includeIf.gitconfig.path
* git config --global --edit  

  
  



