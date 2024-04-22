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
