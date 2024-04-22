# Bundle 1

## Exercise 1

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions  
$ `git init`
Initialized empty Git repository in C:/Users/Think/Desktop/HelloWorld!/Git-Exercise-Solutions/.git/

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (master)
$ `git branch -m master main`

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ `git add .`

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ `git commit -m 'Initial commit'`
[master (root-commit) 5c6bc3c] Initial commit
1 file changed, 0 insertions(+), 0 deletions(-)
create mode 100644 README.md

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (master)
$ git remote add origin https://github.com/Chartine02/Gym-Git-Exercise-Solutions.git

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ `git push -u origin main`
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 214 bytes | 53.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Chartine02/Gym-Git-Exercise-Solutions.git

- [new branch] main -> main
  branch 'main' set up to track 'origin/main'.

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ `git branch dev`

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ git branch
dev

- main

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ git checkout dev
Switched to branch 'dev'

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ `git branch test`

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ `git branch -d test`
Deleted branch test (was 5c6bc3c).

## Exercise 2

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ `git status`
On branch dev
Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: README.md

Untracked files:
(use "git add <file>..." to include in what will be committed)
home.html
Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ `git stash`
Saved working directory and index state WIP on dev: 5c6bc3c Initial commit

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dUntracked files:
(use "git add <file>..." to include in what will be committed)
nothing added to commit but untracked files present (use "git add" to track)
nothing added to commit but untracked files present (use "git add" to track)

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ `git stash`
Saved working directory and index state WIP on dev: 5c6bc3c Initial commit

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: 5c6bc3c Initial commit
stash@{1}: WIP on dev: 5c6bc3c Initial commit

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ `git stash`
No local changes to save

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ `git stash`
Saved working directory and index state WIP on dev: 5c6bc3c Initial commit

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ `git stash list`
stash@{0}: WIP on dev: 5c6bc3c Initial commit
stash@{1}: WIP on dev: 5c6bc3c Initial commit
stash@{2}: WIP on dev: 5c6bc3c Initial commit

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ `git stash pop stash@{2}`
On branch dev
Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)  
 modified: README.md

Untracked files:
(use "git add <file>..." to include in what will be committed)
home.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{2} (eb1e73010100d241be24ac48b57afa819c5dc156)

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ `git stash list`
stash@{0}: WIP on dev: 5c6bc3c Initial commit
stash@{1}: WIP on dev: 5c6bc3c Initial commit

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ `git stash pop stash@{1}`
On branch dev
Changes to be committed:
(use "git restore --staged <file>..." to unstage)
new file: about.html

Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)  
 modified: README.md

Untracked files:
(use "git add <file>..." to include in what will be committed)
home.html

Dropped stash@{1} (9f78114b91f1ca6fc0d67dda9ba8d38ee5251670)

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ `git add .`

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ `git commit -m 'new files in dev'`
[dev c644217] new files in dev
3 files changed, 77 insertions(+)
create mode 100644 about.html
create mode 100644 home.html

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ git push --set-upstream origin dev
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 2 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 1.06 KiB | 83.00 KiB/s, done.
Total 5 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote: https://github.com/Chartine02/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/Chartine02/Gym-Git-Exercise-Solutions.git

- [new branch] dev -> dev
  branch 'dev' set up to track 'origin/dev'.

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ git stash pop
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
(use "git restore --staged <file>..." to unstage)
new file: team.html

$ `git reset`

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$ `git status`
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
(use "git add <file>..." to include in what will be committed)
team.html

nothing added to commit but untracked files present (use "git add" to track)

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (dev)
$

# Bundle 2

## Exercise 1

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ git checkout -b ft/bundle-2
Switched to branch 'ft/bundle-2'

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/bundle-2)
$ git add .

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/bundle-2)
$ git commit -m 'service pages'
[ft/bundle-2 76a35b0] service pages
1 file changed, 11 insertions(+)
t/bundle-2)

$ git push -u origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 447 bytes | 15.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote: https://github.com/Chartine02/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/Chartine02/Gym-Git-Exercise-Solutions.git

- [new branch] ft/bundle-2 -> ft/bundle-2
  branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

## Exercise 2
