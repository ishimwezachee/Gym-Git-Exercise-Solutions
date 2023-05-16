# Gym-Git-Exercise-Solutions
## Bundle 1

### Exercise 1

```bash 
ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions
$ git init
Initialized empty Git repository in C:/Users/ZACHEE/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions/.git/

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git branch -M main

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ touch README.md

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ echo "# Gym-Git-Exercise-Solutions" >> README.md

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ ls
README.md

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git add README.md
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git commit -m "first commit"
[main (root-commit) 2ee733f] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git remote add origin https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 240 bytes | 240.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git checkout -b dev
Switched to a new branch 'dev'

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git push origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git checkout -b test
Switched to a new branch 'test'

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (test)
$ git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions/pull/new/test
remote:
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
 * [new branch]      test -> test

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (test)
$ git checkout dev
Switched to branch 'dev'

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git branch -D test
Deleted branch test (was 2ee733f).

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git push origin --delete test
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
 - [deleted]         test

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)

```
### Exercise 2 

```bash
ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ touch home.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git add .
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: fc771d0 Added exercises 1

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: fc771d0 Added exercises 1

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ touch about.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git add about.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: fc771d0 Added exercises 1

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: fc771d0 Added exercises 1
stash@{1}: WIP on dev: fc771d0 Added exercises 1

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ touch team.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git add team.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: fc771d0 Added exercises 1

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: fc771d0 Added exercises 1
stash@{1}: WIP on dev: fc771d0 Added exercises 1
stash@{2}: WIP on dev: fc771d0 Added exercises 1

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (a995f12bc74ae042fec5af48ea28dc4bdbfd1a90)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped stash@{1} (17ee061ed81cdc6692e44e6df1aaf876a6b2786b)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: fc771d0 Added exercises 1

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md


ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git commit -m "add home and about page"
[dev 161a334] add home and about page
 2 files changed, 24 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 562 bytes | 281.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
   fc771d0..161a334  dev -> dev

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git stash pop
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped refs/stash@{0} (14115fc0959e039b6d5d240e1a4f869628c69eff)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$ git reset --hard
HEAD is now at 161a334 add home and about page

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (dev)
$

```

## Bundle 2 

### Exercise 1 

```bash 
ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ touch services.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git status
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        services.html

nothing added to commit but untracked files present (use "git add" to track)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git add .

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git commit -m 'add services page'
[ft/bundle-2 2caf2cb] add services page
 1 file changed, 12 insertions(+)
 create mode 100644 services.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 475 bytes | 475.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/bundle-2)
$

```


### Exercise 2

```bash
ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git commit -m 'add changes to service page'
[ft/service-redesign 45f6083] add changes to service page
 1 file changed, 5 insertions(+), 1 deletion(-)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 348 bytes | 348.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git add .

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git commit -m 'add changes from main branch'
[main 4bce6af] add changes from main branch
 1 file changed, 8 insertions(+), 1 deletion(-)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git push
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), 638 bytes | 14.00 KiB/s, done.
From https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions
   73f53d3..0b5a2a2  main       -> origin/main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main|MERGING)
$ git status
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 2 different commits each, respectively.  
  (use "git pull" to merge the remote branch into yours)

You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main|MERGING)
$ git add .

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main|MERGING)
$ git commit
[main be335d0] Merge branch 'main' of https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 546 bytes | 546.00 KiB/s, done.
Total 4 (delta 3), reused 0 (delta 0), pack-reused 0        
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
   0b5a2a2..be335d0  main -> main

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
```
