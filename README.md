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
