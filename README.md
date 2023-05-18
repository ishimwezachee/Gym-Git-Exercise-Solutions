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
## Bundle 3 

### Exercise 1 

```bash 
ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/team-page)
$ touch team.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/team-page)
$ git status
On branch ft/team-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/team-page)
$ git add .

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/team-page)
$ git commit -m 'adding team page'
[ft/team-page ded7d45] adding team page
 1 file changed, 12 insertions(+)
 create mode 100644 team.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/team-page)
$  git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 468 bytes | 468.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/team-page)
$ git log
commit ded7d458d8b78dde252793d6282f81e3bc837878 (HEAD -> ft/team-page, origin/ft/team-page)
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 12:19:01 2023 +0200

    adding team page

commit 42a175162dea0fca46de7c515bf978deed90808c (origin/main, main, ft/contact-page)
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 12:10:53 2023 +0200

    add Exercise 2

commit be335d09b9acd078cc2daf2a36468d4988d4ad00
Merge: 4bce6af 0b5a2a2
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 12:05:53 2023 +0200

    Merge branch 'main' of https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions

commit 4bce6af0f6db6ca5e1774046968a32257503682a
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 11:49:28 2023 +0200

    add changes from main branch

commit 0b5a2a26cc2eeddd5d163533afc8c285c44d547e
Merge: 73f53d3 45f6083
Author: zachee ishimwe <zacheeishimwe@gmail.com>
Date:   Tue May 16 11:46:40 2023 +0200

    Merge pull request #2 from ishimwezachee/ft/service-redesign

    Add changes to service page

commit 45f6083d9465024ffd72f0b0ed4d69608645e9fe (origin/ft/service-redesign, ft/service-redesign)
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 11:39:40 2023 +0200

    add changes to service page

commit 73f53d38303efd9dbde036712751c6e307a9ab71
Merge: 2ee733f 622ec30
Author: zachee ishimwe <zacheeishimwe@gmail.com>
Date:   Tue May 16 11:02:19 2023 +0200

    Merge pull request #1 from ishimwezachee/ft/bundle-2

    Add service page

commit 622ec30d24543b917dd446d709c9dd6104a7df61 (origin/ft/bundle-2, ft/bundle-2)
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 10:55:56 2023 +0200

    add exercise1 bundle 2

commit 2caf2cb4843cf13dc924e229a720cccf70d9dcaf
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 10:49:06 2023 +0200

    add services page

commit e2ddd303a3565026709b74342f856cf33e8fe6c2 (origin/dev, dev)
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 10:46:06 2023 +0200

    add exercise 2

commit 161a334d876384d16e44b6a27cdc138c3c5308ed
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 10:42:24 2023 +0200

    add home and about page


ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git cherry-pick ded7d458d8b78dde252793d6282f81e3bc837878
[ft/contact-page 3d5cbff] adding team page
 Date: Tue May 16 12:19:01 2023 +0200
 1 file changed, 12 insertions(+)
 create mode 100644 team.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git touch contact.html
git: 'touch' is not a git command. See 'git --help'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/contact-page)
$ touch contact.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/contact-page)
$ cat contact.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact</title>
</head>
<body>
    <h1>This is contact page</h1>
</body>
</html>
ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git add .

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/contact-page)
$ gi commit -m 'added contact page setup'
bash: gi: command not found

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git commit -m 'added contact page setup'
[ft/contact-page db46238] added contact page setup
 1 file changed, 12 insertions(+)
 create mode 100644 contact.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 741 bytes | 741.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/faq-page)
$ touch faq.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git status
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git add .

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git commit -m 'add faq page'
[ft/faq-page 40ba271] add faq page
 1 file changed, 12 insertions(+)
 create mode 100644 faq.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 449 bytes | 449.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git revert ded7d458d8b78dde252793d6282f81e3bc837878
[ft/faq-page f49d2f4] Revert "adding team page"
 1 file changed, 12 deletions(-)
 delete mode 100644 team.html

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 274 bytes | 274.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
   40ba271..f49d2f4  ft/faq-page -> ft/faq-page

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/faq-page)
```

### Exercises 2

```bash

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
* ft/faq-page
  ft/service-redesign
  ft/team-page
  main

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/faq-page)
$

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
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
        modified:   about.html
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git add .

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git commit -m 'added main and footer to pages'
[main 4aaace4] added main and footer to pages
 2 files changed, 4 insertions(+)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 455 bytes | 455.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
   b896cb6..4aaace4  main -> main

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git log
commit f49d2f459d87b7b4e517df91e30863fcebb032c0 (HEAD -> ft/home-page-redesign, origin/ft/faq-page, ft/faq-page)
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 12:38:42 2023 +0200

    Revert "adding team page"

    This reverts commit ded7d458d8b78dde252793d6282f81e3bc837878.

commit 40ba271c0663ac67533b27d34676284725acd0de
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 12:36:30 2023 +0200

    add faq page

commit db4623851ad5fd2e7f46b351ecd051bf23fef946 (origin/ft/contact-page, ft/contact-page)
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 12:32:44 2023 +0200

    added contact page setup

commit 3d5cbffbacaff7fa4533ac877fe602976d99059a
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 12:19:01 2023 +0200

    adding team page

commit 42a175162dea0fca46de7c515bf978deed90808c
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 12:10:53 2023 +0200

    add Exercise 2

commit be335d09b9acd078cc2daf2a36468d4988d4ad00
Merge: 4bce6af 0b5a2a2
Author: ishimwezachee <zacheeishimwe@gmail.com>
Date:   Tue May 16 12:05:53 2023 +0200

    Merge branch 'main' of https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git add .

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git commit -m 'add changes to home pages'
[ft/home-page-redesign 060cd8b] add changes to home pages
 1 file changed, 6 insertions(+), 2 deletions(-)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign

Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 4 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (14/14), 1.59 KiB | 815.00 KiB/s, done.
Total 14 (delta 7), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (7/7), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
```

## Bundle 4

### Exercise 1

```bash 
ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git remote add git-copy https://github.com/ishimwezachee/git-exercise-clone.git

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git remote
git-copy
origin

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git commit -m 'content to main in home page'
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git add .

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git commit -m 'content to main in home page'
[main a7d0c91] content to main in home page
 1 file changed, 3 insertions(+), 1 deletion(-)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git push origin
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 344 bytes | 344.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
   cac191a..a7d0c91  main -> main

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git push git-copy
Enumerating objects: 44, done.
Counting objects: 100% (44/44), done.
Delta compression using up to 4 threads
Compressing objects: 100% (41/41), done.
Writing objects: 100% (44/44), 9.81 KiB | 436.00 KiB/s, done.
Total 44 (delta 18), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (18/18), done.
To https://github.com/ishimwezachee/git-exercise-clone.git
 * [new branch]      main -> main

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
```

### Exercise 3
```bash
ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/footer)
$ git status
On branch ft/footer
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/footer)
$ git add .

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/footer)
$ git commit -m 'give content to home footer'
[ft/footer 9c78a4a] give content to home footer
 1 file changed, 3 insertions(+), 1 deletion(-)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/footer)
$ git add .

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/footer)
$ git commit -m 'give some content to about footer'
[ft/footer 345cebb] give some content to about footer
 1 file changed, 3 insertions(+), 1 deletion(-)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/footer)
$ git push
fatal: The current branch ft/footer has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/footer

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/footer)
$  git push --set-upstream origin ft/footer
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 714 bytes | 714.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions/pull/new/ft/footer
remote:
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/footer)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/squashing)
$ git merge squash ft/f
ft/faq-page   ft/footer

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/squashing)
$ git merge squash ft/footer
merge: squash - not something we can merge

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/squashing)
$ git merge --squash ft/footer
Updating 0c62030..345cebb
Fast-forward
Squash commit -- not updating HEAD
 about.html | 4 +++-
 home.html  | 4 +++-
 2 files changed, 6 insertions(+), 2 deletions(-)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/squashing)
$ git status
On branch ft/squashing
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   about.html
        modified:   home.html


ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/squashing)
$ git commit -m 'footer changes squashing'
[ft/squashing 60d610b] footer changes squashing
 2 files changed, 6 insertions(+), 2 deletions(-)

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/squashing)
$ git push
fatal: The current branch ft/squashing has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/squashing

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/squashing)
$  git push --set-upstream origin ft/squashing
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 497 bytes | 497.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions/pull/new/ft/squashing
remote:
To https://github.com/ishimwezachee/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/squashing -> ft/squashing
branch 'ft/squashing' set up to track 'origin/ft/squashing'.

ZACHEE@DESKTOP-JM7SBUV MINGW64 ~/Desktop/thegym/trainings/Gym-Git-Exercise-Solutions (ft/squashing)
```
