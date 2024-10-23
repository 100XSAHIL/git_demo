installation
* windows : https://git-scm.com/download/win
* macos: https://sourceforge.net/projects/git-osx-installer/
* linux : https://www.git-scm.com/download/linux
setup
check whether you git is installed or not
git --version
config addition -> name , email
list of configs
git config --list
add your username and your email id
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
how git stores the changes
git has three areas -> working directory-> current changes
Intermeediate layer -> staging
Terms
Repository (Repo): A storage location for your project, including all the files and the entire history of their changes.

staging area -> tracked changes working directory -> untracked changes

git workflow
git init -> wherever you enter git init an empty git repository is created (tracker without any history)
git add -> added to staging area(snapshot of the code is added)
.gitignore : this the file where you can put the files and folder name which you don't want to be tracked
git add . -> to send all the files current snapshot to staging area
git status -> differenece between staging and working directory
git commit -m "commit message"  : A snapshot of changes made to the repository. Each commit has a unique ID and a message describing the changes.
git log : list of commits
git checkout commit-hash : you can view how code looked like in a particular commit
to go back to latest commit -> HEAD
type git branch -> check your branch name
git checkout branch-name
commands to push your changes
Setup remote repo

create a repo in github
git remote add origin remote-repo-name
git branch -M main
git push -u origin main