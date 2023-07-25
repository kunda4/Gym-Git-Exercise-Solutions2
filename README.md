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
## Bundle 1
### Exercise2
```
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ touch home.html
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add home.html
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash push home.html
Saved working directory and index state WIP on dev: 33c43da git exercices first bundle
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash list
stash@{0}: WIP on dev: 33c43da git exercices first bundle
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ touch about.html
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add about.html
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash push about.html
Saved working directory and index state WIP on dev: 33c43da git exercices first bundle
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash list
stash@{0}: WIP on dev: 33c43da git exercices first bundle
stash@{1}: WIP on dev: 33c43da git exercices first bundle
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ touch team.html
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add team.html
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash push team.html
Saved working directory and index state WIP on dev: 33c43da git exercices first bundle
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash list
stash@{0}: WIP on dev: 33c43da git exercices first bundle
stash@{1}: WIP on dev: 33c43da git exercices first bundle
stash@{2}: WIP on dev: 33c43da git exercices first bundle
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (cf143b65c020cad0f134fe205e5966c2d00d6c2d)
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash apply --index stash@{0}
error: Your local changes to the following files would be overwritten by merge:
  about.html
Index was not unstashed.
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash list
stash@{0}: WIP on dev: 33c43da git exercices first bundle
stash@{1}: WIP on dev: 33c43da git exercices first bundle
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash apply --index stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash push team.html
Saved working directory and index state WIP on dev: 33c43da git exercices first bundle
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash list
stash@{0}: WIP on dev: 33c43da git exercices first bundle
stash@{1}: WIP on dev: 33c43da git exercices first bundle
stash@{2}: WIP on dev: 33c43da git exercices first bundle
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash apply --index stash@{2}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit -m " restore home with index"
[dev c45bf23]  restore home with index
 2 files changed, 20 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 544 bytes | 544.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/kunda4/git-exercices2.git
   33c43da..c45bf23  dev -> dev
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash list
stash@{0}: WIP on dev: 33c43da git exercices first bundle
stash@{1}: WIP on dev: 33c43da git exercices first bundle
stash@{2}: WIP on dev: 33c43da git exercices first bundle
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{1} (a29950b3a3983e395fccedc76549c70c5f2d760e)
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git log
commit c45bf2315e702465b6d2f955e7c753c8bfc152d2 (HEAD -> dev, origin/dev)
Author: Agnes IRADUKUNDA <101483232+kunda4@users.noreply.github.com>
Date:   Tue Jul 25 13:08:57 2023 +0200

     restore home with index

commit 33c43dab24c6762cf311ad63fcb0ca3d0d776b00 (origin/main, main)
Author: Agnes IRADUKUNDA <101483232+kunda4@users.noreply.github.com>
Date:   Tue Jul 25 12:32:05 2023 +0200

    git exercices first bundle
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git reset --hard <restore home with index>
bash: syntax error near unexpected token `newline'
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git reset --hard stash@{0}
HEAD is now at 5370aa7 WIP on dev: 33c43da git exercices first bundle
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash list
stash@{0}: WIP on dev: 33c43da git exercices first bundle
stash@{1}: WIP on dev: 33c43da git exercices first bundle
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git stash pop stash@{1}
```
