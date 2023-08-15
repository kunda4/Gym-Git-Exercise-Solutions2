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
## Bundle 2
### Exercice 1
```bash
Andelas-MBP:git-exercises andelarwanda$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
Andelas-MBP:git-exercises andelarwanda$ touch services.html
Andelas-MBP:git-exercises andelarwanda$ git add .
Andelas-MBP:git-exercises andelarwanda$ git commit -m "add services.html file"
[ft/bundle-2 a4a372a] add services.html file
 1 file changed, 12 insertions(+)
 create mode 100644 services.html
Andelas-MBP:git-exercises andelarwanda$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Andelas-MBP:git-exercises andelarwanda$  git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 486 bytes | 486.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/kunda4/git-exercises/pull/new/ft/bundle-2
remote: 
To https://github.com/kunda4/git-exercises.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```
## Bundle 2
### Exercice 2
```
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git pull
remote: Enumerating objects: 2, done.
remote: Counting objects: 100% (2/2), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (2/2), 1.26 KiB | 429.00 KiB/s, done.
From https://github.com/kunda4/git-exercices2
   33c43da..27e7ddf  main       -> origin/main
Updating 33c43da..27e7ddf
Fast-forward
 home.html     | 10 ++++++++++
 services.html | 10 ++++++++++
 team.html     | 10 ++++++++++
 3 files changed, 30 insertions(+)
 create mode 100644 home.html
 create mode 100644 services.html
 create mode 100644 team.html
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit -m "new changes to services.html"
On branch ft/service-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push --set-upstream origin ft/service-redesign
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/kunda4/git-exercices2/pull/new/ft/service-redesign
remote: 
To https://github.com/kunda4/git-exercices2.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit --amend --no-edit
[ft/service-redesign b628c2f] Merge pull request #2 from kunda4/ft/bundle-2
 Author: Ibrahim Bagalwa <67462827+IbrahimBagalwa@users.noreply.github.com>
 Date: Thu Jul 27 20:06:27 2023 +0200
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push --set-upstream origin ft/service-redesign
To https://github.com/kunda4/git-exercices2.git
 ! [rejected]        ft/service-redesign -> ft/service-redesign (non-fast-forward)
error: failed to push some refs to 'https://github.com/kunda4/git-exercices2.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push --set-upstream origin ft/service-redesign --force
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 572 bytes | 572.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/kunda4/git-exercices2.git
 + 27e7ddf...b628c2f ft/service-redesign -> ft/service-redesign (forced update)
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit -m "change on main"
[main cd374dd] change on main
 1 file changed, 5 insertions(+)
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push --set-upstream origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 466 bytes | 466.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/kunda4/git-exercices2.git
   27e7ddf..cd374dd  main -> main
branch 'main' set up to track 'origin/main'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git diff main..ft/service-redesign
diff --git a/services.html b/services.html
index b198148..17f5d4a 100644
--- a/services.html
+++ b/services.html
@@ -7,9 +7,9 @@
 <body>
     <h1>services</h1>
     <ul>
-        <li><a href="about"></a></li>
-        <li><a href="about"></a></li>
-        <li><a href="about"></a></li>
+        <li><a href="#">Home</a></li>
+        <li><a href="#">Home</a></li>
+        <li><a href="#">Home</a></li>
     </ul>
 </body>
 </html>
\ No newline at end of file
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git merge origin main
merge: origin - not something we can merge
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git merge --continue
[ft/service-redesign 6a374a1] Merge branch 'main' into ft/service-redesign
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit --amend --no-edit
[ft/service-redesign bdd934d] Merge branch 'main' into ft/service-redesign
 Date: Fri Jul 28 19:15:21 2023 +0200
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 392 bytes | 392.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/kunda4/git-exercices2.git
   b628c2f..bdd934d  ft/service-redesign -> ft/service-redesign
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ 
```
## Bundle 3
### Exercice 1
```
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ touch team.html
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit -m "new page"
On branch ft/team-page
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit -m "new page"
[ft/team-page 059f7fc] new page
 1 file changed, 1 insertion(+), 1 deletion(-)
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push --set-upstream origin ft/team-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 337 bytes | 337.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/kunda4/git-exercices2/pull/new/ft/team-page
remote: 
To https://github.com/kunda4/git-exercices2.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git log
commit 059f7fc0c3c2769e04166a28dd1a7798717124d5 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Agnes IRADUKUNDA <101483232+kunda4@users.noreply.github.com>
Date:   Tue Aug 1 12:44:01 2023 +0200

    new page

commit bdd934d32a8789290b63f3e4f119053e780260ab (origin/ft/service-redesign, ft/service-redesign)
Merge: b628c2f cd374dd
Author: Agnes IRADUKUNDA <101483232+kunda4@users.noreply.github.com>
Date:   Fri Jul 28 19:15:21 2023 +0200

    Merge branch 'main' into ft/service-redesign

commit cd374dd73fb12e0328a2048406f8fc60eb87a2ef (origin/main, main, ft/contact-page)
Author: Agnes IRADUKUNDA <101483232+kunda4@users.noreply.github.com>
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git cherry-pick 059f7fc0c3c2769e04166a28dd1a7798717124d5
[ft/contact-page c64fb3b] new page
 Date: Tue Aug 1 12:44:01 2023 +0200
 1 file changed, 1 insertion(+), 1 deletion(-)
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit -m "add last commit"
On branch ft/contact-page
nothing to commit, working tree clean
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$  git push --set-upstream origin ft/contact-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 342 bytes | 342.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/kunda4/git-exercices2/pull/new/ft/contact-page
remote: 
To https://github.com/kunda4/git-exercices2.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ touch faq.html
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit -m "new faq.html file"
[ft/faq-page ae4339f] new faq.html file
 1 file changed, 10 insertions(+)
 create mode 100644 faq.html
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 453 bytes | 453.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/kunda4/git-exercices2/pull/new/ft/faq-page
remote: 
To https://github.com/kunda4/git-exercices2.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git revert 059f7fc0c3c2769e04166a28dd1a7798717124d5
[ft/faq-page 5b3da2b] Revert "new page"
 1 file changed, 1 insertion(+), 1 deletion(-)
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit -m "revert"
On branch ft/faq-page
Your branch is ahead of 'origin/ft/faq-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 373 bytes | 373.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/kunda4/git-exercices2.git
   ae4339f..5b3da2b  ft/faq-page -> ft/faq-page
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ 
```
## Bundle 3
### Exercice 2
```
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit -m "make changes on main"
[main 4e68d68] make changes on main
 1 file changed, 5 insertions(+)
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git rebase main
Auto-merging team.html
CONFLICT (content): Merge conflict in team.html
error: could not apply c64fb3b... new page
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
Could not apply c64fb3b... new page
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git status
interactive rebase in progress; onto 4e68d68
Last command done (1 command done):
   pick c64fb3b new page
Next commands to do (2 remaining commands):
   pick ae4339f new faq.html file
   pick 5b3da2b Revert "new page"
  (use "git rebase --edit-todo" to view and edit)
You are currently rebasing branch 'ft/home-page-redesign' on '4e68d68'.
  (fix conflicts and then run "git rebase --continue")
  (use "git rebase --skip" to skip this patch)
  (use "git rebase --abort" to check out the original branch)

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git rebase --continue
[detached HEAD de725b4] new page
 1 file changed, 1 insertion(+)
Auto-merging team.html
CONFLICT (content): Merge conflict in team.html
error: could not apply 5b3da2b... Revert "new page"
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
Could not apply 5b3da2b... Revert "new page"
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git rebase --continue
Successfully rebased and updated refs/heads/ft/home-page-redesign.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git rebase --continue
fatal: No rebase in progress?
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git status
On branch ft/home-page-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git status
On branch ft/home-page-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   home.html

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit -m"add change to home page"
[ft/home-page-redesign 355ddb9] add change to home page
 1 file changed, 5 insertions(+)
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$  git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 15, done.
Counting objects: 100% (15/15), done.
Delta compression using up to 4 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (12/12), 1.48 KiB | 378.00 KiB/s, done.
Total 12 (delta 6), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (6/6), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/kunda4/git-exercices2/pull/new/ft/home-page-redesign
remote: 
To https://github.com/kunda4/git-exercices2.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ 
```
## Bundle 4
### Exercice 1
```bash
Andelas-MBP:git-exercises andelarwanda$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Andelas-MBP:git-exercises andelarwanda$ git remote add git-copy https://github.com/kunda4/git-exercises-clone.git
Andelas-MBP:git-exercises andelarwanda$ git remote
git-copy
origin
Andelas-MBP:git-exercises andelarwanda$ git add .
Andelas-MBP:git-exercises andelarwanda$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   home.html

Andelas-MBP:git-exercises andelarwanda$ git commit -m "modify home.html"
[main c37fadc] modify home.html
 1 file changed, 1 insertion(+)
Andelas-MBP:git-exercises andelarwanda$ git push origin
To https://github.com/kunda4/git-exercises.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/kunda4/git-exercises.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
Andelas-MBP:git-exercises andelarwanda$ git push -u git-copy main
Enumerating objects: 21, done.
Counting objects: 100% (21/21), done.
Delta compression using up to 2 threads
Compressing objects: 100% (19/19), done.
Writing objects: 100% (21/21), 2.92 KiB | 1.46 MiB/s, done.
Total 21 (delta 12), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (12/12), done.
To https://github.com/kunda4/git-exercises-clone.git
 * [new branch]      main -> main
Andelas-MBP:git-exercises andelarwanda$ git push -u origin main
To https://github.com/kunda4/git-exercises.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/kunda4/git-exercises.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
Andelas-MBP:git-exercises andelarwanda$ git push origin --force
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 340 bytes | 340.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/kunda4/git-exercises.git
 + a3fff70...c37fadc main -> main (forced update)
Andelas-MBP:git-exercises andelarwanda$ 
```
## Bundle 4
### Exercice 2
```bash
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit -m "add a paragraph"
On branch ft/footer
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit -m "add header"
[ft/footer a5007cd] add header
 1 file changed, 5 insertions(+)
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push -u origin ft/footer
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 522 bytes | 522.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/kunda4/git-exercices2/pull/new/ft/footer
remote: 
To https://github.com/kunda4/git-exercices2.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'git-copy/main'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'git-copy/main'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git checkout ft/squashing
Switched to branch 'ft/squashing'
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$  git merge --squash ft/footer
Updating 50622f0..a5007cd
Fast-forward
Squash commit -- not updating HEAD
 home.html | 5 +++++
 1 file changed, 5 insertions(+)
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git add .
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git commit -m "footer changes squashing"
[ft/squashing e105ce6] footer changes squashing
 1 file changed, 5 insertions(+)
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push 
fatal: The current branch ft/squashing has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/squashing

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ git push --set-upstream origin ft/squashing
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 535 bytes | 535.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/kunda4/git-exercices2/pull/new/ft/squashing
remote: 
To https://github.com/kunda4/git-exercices2.git
 * [new branch]      ft/squashing -> ft/squashing
branch 'ft/squashing' set up to track 'origin/ft/squashing'.
Andelas-MacBook-Pro:git-exrcises2 andelarwanda$ 
```
## Bundle 5
### Exercice 2
```bash
Andelas-MacBook-Pro:git-cafe-exercise andelarwanda$ git add .
Andelas-MacBook-Pro:git-cafe-exercise andelarwanda$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   index.html

Andelas-MacBook-Pro:git-cafe-exercise andelarwanda$ git commit -m "change place to restaurent"
[main e71efea] change place to restaurent
 1 file changed, 1 insertion(+), 1 deletion(-)
Andelas-MacBook-Pro:git-cafe-exercise andelarwanda$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 357 bytes | 357.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/kunda4/git-cafe-exercise.git
   d1d3f9c..e71efea  main -> main
```
## Bundle 6
### Exercice 1
```bash
Andelas-MacBook-Pro:git-cafe-exercise andelarwanda$ git checkout -b ft/new-branch
Switched to a new branch 'ft/new-branch'
Andelas-MacBook-Pro:git-cafe-exercise andelarwanda$ touch menu.html
Andelas-MacBook-Pro:git-cafe-exercise andelarwanda$ git add .
Andelas-MacBook-Pro:git-cafe-exercise andelarwanda$ git commit -m "add new change to menu"
[ft/new-branch f94a552] add new change to menu
 1 file changed, 14 insertions(+)
 create mode 100644 menu.html
Andelas-MacBook-Pro:git-cafe-exercise andelarwanda$ git push
fatal: The current branch ft/new-branch has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/new-branch

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Andelas-MacBook-Pro:git-cafe-exercise andelarwanda$ 
Andelas-MacBook-Pro:git-cafe-exercise andelarwanda$    git push --set-upstream origin ft/new-branch
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 485 bytes | 485.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/new-branch' on GitHub by visiting:
remote:      https://github.com/kunda4/git-cafe-exercise/pull/new/ft/new-branch
remote: 
To https://github.com/kunda4/git-cafe-exercise.git
 * [new branch]      ft/new-branch -> ft/new-branch
branch 'ft/new-branch' set up to track 'origin/ft/new-branch'.
Andelas-MacBook-Pro:git-cafe-exercise andelarwanda$ 
```
