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

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 3 commits.
(use "git push" to publish your local commits)

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
(use "git push" to publish your local commits)

Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: README.md
modified: services.html

no changes added to commit (use "git add" and/or "git commit -a")

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ git add .

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ git push -u origin main
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1008 bytes | 144.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Chartine02/Gym-Git-Exercise-Solutions.git
90c4321..9d5b510 main -> main
branch 'main' set up to track 'origin/main'.

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

Merge branch 'main' into ft/service-redesign
Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/service-redesign|MERGING)
$ git add .

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/service-redesign|MERGING)
$ git commit
[ft/service-redesign 36b4384] Merge branch 'main' into ft/service-redesign

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/service-redesign)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 272 bytes | 90.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Chartine02/Gym-Git-Exercise-Solutions.git
9ad4fb9..36b4384 ft/service-redesign -> ft/service-redesign

# Bundle 3

## Exercise 1

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ git branch ft/team-page

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/team-page)
$ git add .

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/team-page)
$ git commit -m 'ft-team page'
[ft/team-page 46c620f] ft-team page
1 file changed, 1 insertion(+), 1 deletion(-)

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 323 bytes | 323.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote: https://github.com/Chartine02/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/Chartine02/Gym-Git-Exercise-Solutions.git

- [new branch] ft/team-page -> ft/team-page
  branch 'ft/team-page' set up to track 'origin/ft/team-page'.

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ git branch ft/contact-page

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (main)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/team-page)
$ git log
commit 46c620f1e059de576bdc6c23dbe58f109666d935 (HEAD -> ft/team-page, origin/ft/team-page)
Author: chartine02 <noellachartine125@gmail.com>
Date: Mon Apr 22 19:36:36 2024 +0200

    ft-team page

commit 22434195fc37fc788523bc2f5bf0a601e0efb784 (origin/main, main, ft/contact-page)
Author: chartine02 <noellachartine125@gmail.com>
Date: Mon Apr 22 19:31:40 2024 +0200

    updated readme

commit 9d5b5105defc9eff8694aed77d561d0aae7f39e3
Author: chartine02 <noellachartine125@gmail.com>
Date: Mon Apr 22 17:31:53 2024 +0200

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/contact-page)
$ git cherry-pick 46c620f1e059de576bdc6c23dbe58f109666d935
[ft/contact-page 4ab471a] ft-team page
Date: Mon Apr 22 19:36:36 2024 +0200
1 file changed, 1 insertion(+), 1 deletion(-)

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/contact-page)
$ git add .

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/contact-page)
$ git status
On branch ft/contact-page
Untracked files:
(use "git add <file>..." to include in what will be committed)
contact.html

nothing added to commit but untracked files present (use "git add" to track)

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/contact-page)
$ git addv.
git: 'addv.' is not a git command. See 'git --help'.

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/contact-page)
$ git add .

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/contact-page)
$ git commit -m ' ft-contact page '
[ft/contact-page 13e30f3] ft-contact page
1 file changed, 11 insertions(+)
create mode 100644 contact.html

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 2 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 752 bytes | 107.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote: https://github.com/Chartine02/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/Chartine02/Gym-Git-Exercise-Solutions.git

- [new branch] ft/contact-page -> ft/contact-page
  branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/faq-page)
$ git add .

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/faq-page)
$ git commit -m 'ft-faq page'
[ft/faq-page aada8d9] ft-faq page
1 file changed, 11 insertions(+)
create mode 100644 faq.html

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Revert "ft-team page"
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 426 bytes | 71.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote: https://github.com/Chartine02/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/Chartine02/Gym-Git-Exercise-Solutions.git

- [new branch] ft/faq-page -> ft/faq-page
  branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/faq-page)
$ git revert 46c620f1e059de576bdc6c23dbe58f109666d935
[ft/faq-page 08391ce] Revert "ft-team page"
1 file changed, 1 insertion(+), 1 deletion(-)

Think@DESKTOP-96IITAO MINGW64 ~/Desktop/HelloWorld!/Git-Exercise-Solutions (ft/faq-page)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 347 bytes | 173.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Chartine02/Gym-Git-Exercise-Solutions.git
aada8d9..08391ce ft/faq-page -> ft/faq-page
