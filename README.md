# Gym-Git-Exercise-Solutions2
## Bundle 1
### Exercise1
```
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git init
Initialized empty Git repository in /Users/andelarwanda/Desktop/TheGym/git-exrcises2/.git/
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git branch -m main master
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git branch -m master main 
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git status
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ touch file1.txt file2.txt file3.txt
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file1.txt
        file2.txt
        file3.txt

nothing added to commit but untracked files present (use "git add" to track)
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   file1.txt
        new file:   file2.txt
        new file:   file3.txt

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ mv file1.txt file11.txt
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ mv file2.txt file22.txt
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ mv file3.txt file33.txt
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   file1.txt
        new file:   file2.txt
        new file:   file3.txt

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    file1.txt
        deleted:    file2.txt
        deleted:    file3.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file11.txt
        file22.txt
        file33.txt

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   file11.txt
        new file:   file22.txt
        new file:   file33.txt

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit -m "git exercices first bundle"
[main (root-commit) 33c43da] git exercices first bundle
 3 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 file11.txt
 create mode 100644 file22.txt
 create mode 100644 file33.txt
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git remote add origin https://github.com/kunda4/git-exercices2.git
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$  git push --set-upstream origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 261 bytes | 65.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/kunda4/git-exercices2.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git branch checkout -b dev
error: unknown switch `b'

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout -b dev
Switched to a new branch 'dev'
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout -b test
Switched to a new branch 'test'
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout dev
Switched to branch 'dev'
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git branch -d test
Deleted branch test (was 33c43da).
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$
```
