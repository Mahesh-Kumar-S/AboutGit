# AboutGit

Git pull - pulling code from Remote repository to Working space directory
Git Fetch - Copy from Remote repository to local git repo
Git Merge - Copy from local git repository to Working space directory

Git pull=git fetch + git merge

Steps:
1. git clone 
2. git checkout
3. git add to staging
4. git commit to local repo
5. git push to feature branch
6. git merge with PR

Steps in command line git bash:
1. git init
3. git status (changes to be added will be shown-shows in red color)
4. git add (to add the changes)
5. git status (changes added will be listed-shows in green color)
6. git commit -m "something written here"
7. git remote add origin url of remote repo
8. git push origin master

git stash (erasing the added values in staging area)
git revert 
git checkout branch name (switching to another branch)

---
if this error occurs in git
$ git commit -m “version 1”
On branch master
Your branch is up to date with ‘origin/master’.
nothing to commit, working tree clean

git init doesn’t initialize if you already have a .git/ folder in your repository. So, for your case, do -

(1) rm -rf .git/

(2) git init

(3) git remote add origin https://repository.remote.url 703

(4) git commit -m “Commit message”

(5) git push -f origin master

--
 git log --diff-filter=D --summary  (to find the deleted files)
 
--
If you deelted the file and restioe to back

  git reset HEAD~ (Undo commit and unstage all files)
  
  git status
  
  git restore filename
  
  How do you do this for multiple deleted files? - git reset HEAD \* and then git checkout -- .
  
  
  https://bytefreaks.net/programming-2/how-to-undo-a-git-commit-that-was-not-pushed
  
  https://stackoverflow.com/questions/11956710/git-recover-deleted-file-where-no-commit-was-made-after-the-delete
  
 
