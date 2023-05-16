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

