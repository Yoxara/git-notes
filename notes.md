__Author identity unknown__
Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in one repository.


__create a new repository:__
git ini <repository>

__checkout a repository:__
git clone /path/to/repository
using the remote server: git clone username@host:/path/to/repository


__workflow: add & commit__
git add <repository>
git add *
git commit -m "Commit message"

    
__pushing changes:__
git push origin master
Remote server: git remote add origin <server>

    
__branching:__
create a new branch: git checkout -b <branch>
switch back to master: git checkout master
delete the branch: git branch -d <branch>
a branch is not available to others unless you push the branch to your remote repository: git push origin <branch>


__update & merge__
update your local repository to the newest commit: git pull
to merge another branch into your active branch: git merge <branch>
After changing, you need to mark them as merged with: git add <repository>
before merging changes, you can also preview them by using: git diff <source_branch> <target_branch>

   
__tagging__
You can create a new tag named 1.0.0 by executing: git tag 1.0.0 1b2e1d63ff
1b2e1d63ff stands for the first 10 characters of the commit id you want to reference with your tag. 
    
    
__log__
you can study repository history using: git log
To see only the commits of a certain author: git log --author=bob
To see a very compressed log where each commit is one line: git log --pretty=oneline
Or maybe you want to see an ASCII art tree of all the branches, decorated with the names of tags and branches:
git log --graph --oneline --decorate --all
See only which files have changed: git log --name-status
For more, see git log --help    
    
    
__replace local changes__
you can replace local changes using the command: git checkout -- <filename>
If you instead want to drop all your local changes and commits, fetch the latest history from the server and point your local master branch at it like this:
git fetch origin
git reset --hard origin/master    
    
    
__useful hints__
built-in git GUI: gitk
use colorful git output: git config color.ui true
show log on just one line per commit: git config format.pretty oneline
use interactive adding: git add -i
    
    
__Reference__
https://rogerdudler.github.io/git-guide/
    

Summary:

…or create a new repository on the command line

echo "# repository" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/User/repository.git
git push -u origin main

…or push an existing repository from the command line

git remote add origin https://github.com/User/repository.git
git branch -M main
git push -u origin main





Quick setup — if you’ve done this kind of thing before
or	
https://github.com/Yoxara/name.git
Get started by creating a new file or uploading an existing file. We recommend every repository include a README, LICENSE, and .gitignore.

…or create a new repository on the command line
echo "# name" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/Yoxara/name.git
git push -u origin main
…or push an existing repository from the command line
git remote add origin https://github.com/Yoxara/name.git
git branch -M main
git push -u origin main
