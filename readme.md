# Git exercises 1

## Exercise one
```bash
LONOVO@toussaintn23 MINGW64 ~/Git Exercises
$ git init 
Initialized empty Git repository in C:/Users/LONOVO/Git Exercises/.git/

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (master)
$ git branch -M main

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git status
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.md

nothing added to commit but untracked files present (use "git add" to track)

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git add .

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git commit -m "This is the exercise 1"
[main (root-commit) 47826cf] This is the exercise 1
 1 file changed, 3 insertions(+)
 create mode 100644 readme.md

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git remote add origin https://github.com/tnkundwa/Gym-Git-Exercise-Solutions.git

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git status
On branch main
nothing to commit, working tree clean

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git push --set-upstream origin main
To https://github.com/tnkundwa/Gym-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/tnkundwa/Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git pull origin main
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 915 bytes | 53.00 KiB/s, done.
From https://github.com/tnkundwa/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
fatal: refusing to merge unrelated histories

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git add .

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git commit -m "Merge remote changes"
On branch main
nothing to commit, working tree clean

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git push --set-upstream origin main
To https://github.com/tnkundwa/Gym-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/tnkundwa/Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. If you want to integrate the remote changes,
hint: use 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git push --force --set-upstream origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 281 bytes | 281.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/tnkundwa/Gym-Git-Exercise-Solutions.git
 + 50ac350...47826cf main -> main (forced update)
branch 'main' set up to track 'origin/main'.

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git push
Everything up-to-date

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/bundle-2)
$ git status
On branch ft/bundle-2
nothing to commit, working tree clean

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/tnkundwa/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/tnkundwa/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/bundle-2)
$ git push
Everything up-to-date

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/bundle-2)
$ git branch -m "ft/bundle-2" "dev"

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git branch
* dev
  main

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/ft/bundle-2'.

nothing to commit, working tree clean

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git push
fatal: The upstream branch of your current branch does not match
the name of your current branch.  To push to the upstream branch
on the remote, use

    git push origin HEAD:ft/bundle-2

To push to the branch of the same name on the remote, use

    git push origin HEAD

To choose either option permanently, see push.default in 'git help config'.

To avoid automatically configuring an upstream branch when its name
won't match the local branch, see option 'simple' of branch.autoSetupMerge
in 'git help config'.


LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git push
fatal: The upstream branch of your current branch does not match
the name of your current branch.  To push to the upstream branch
on the remote, use

    git push origin HEAD:ft/bundle-2

To push to the branch of the same name on the remote, use

    git push origin HEAD

To choose either option permanently, see push.default in 'git help config'.

To avoid automatically configuring an upstream branch when its name
won't match the local branch, see option 'simple' of branch.autoSetupMerge
in 'git help config'.


LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git branch
* dev
  main

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ bit status
bash: bit: command not found

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/ft/bundle-2'.

nothing to commit, working tree clean

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git push origin "dev"
Everything up-to-date

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git push
fatal: The upstream branch of your current branch does not match
the name of your current branch.  To push to the upstream branch
on the remote, use

    git push origin HEAD:ft/bundle-2

To push to the branch of the same name on the remote, use

    git push origin HEAD

To choose either option permanently, see push.default in 'git help config'.

To avoid automatically configuring an upstream branch when its name
won't match the local branch, see option 'simple' of branch.autoSetupMerge
in 'git help config'.


LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git branch
* dev
  main

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git checkout -b Test
Switched to a new branch 'Test'

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (Test)
$ git push origin test
fatal: test cannot be resolved to branch

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (Test)
$ git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/ft/bundle-2'.

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git delete -D test
git: 'delete' is not a git command. See 'git --help'.

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git branch -D test
Deleted branch test (was 47826cf).

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git push origin --delete test
error: unable to delete 'test': remote ref does not exist
error: failed to push some refs to 'https://github.com/tnkundwa/Gym-Git-Exercise-Solutions.git'

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git branch
* dev
  main

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (dev)
$ git checkout main
M       readme.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```

##Exercise 2
```bash
LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git pull
Your configuration specifies to merge with the ref 'refs/heads/ft/bundle-2'
from the remote, but no such ref was fetched.

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/ft/bundle-2'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html


LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git add home.html

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git stash
Saved working directory and index state WIP on dev: 47826cf This is the exercise 1

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git stash list
stash@{0}: WIP on dev: 47826cf This is the exercise 1

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git add about.html 

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git stash
Saved working directory and index state WIP on dev: 47826cf This is the exercise 1

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/ft/bundle-2'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git add team.html 

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git stash
Saved working directory and index state WIP on dev: 47826cf This is the exercise 1

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git stash list
stash@{0}: WIP on dev: 47826cf This is the exercise 1
stash@{1}: WIP on dev: 47826cf This is the exercise 1
stash@{2}: WIP on dev: 47826cf This is the exercise 1

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/ft/bundle-2'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (e2a12f3cc3a42921623df1d59ade9c5280fa8cd6)

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git stash list
stash@{0}: WIP on dev: 47826cf This is the exercise 1
stash@{1}: WIP on dev: 47826cf This is the exercise 1

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/ft/bundle-2'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html

Dropped stash@{0} (598a38caccc3a5a67f4d0f1fe1e6a64ac7d95544)

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$  git status
On branch dev
Your branch is up to date with 'origin/ft/bundle-2'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html


LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git add .

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git commit -m "This is the home and team"
[dev d226dbf] This is the home and team
 2 files changed, 22 insertions(+)
 create mode 100644 about.html
 create mode 100644 team.html

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git push
fatal: The upstream branch of your current branch does not match
the name of your current branch.  To push to the upstream branch
on the remote, use

    git push origin HEAD:ft/bundle-2

To push to the branch of the same name on the remote, use

    git push origin HEAD

To choose either option permanently, see push.default in 'git help config'.

To avoid automatically configuring an upstream branch when its name
won't match the local branch, see option 'simple' of branch.autoSetupMerge
in 'git help config'.


LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git merge ft/bundle-2
merge: ft/bundle-2 - not something we can merge

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git push origin HEAD:ft/bundle-2
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 550 bytes | 550.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/tnkundwa/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
remote: Heads up! The branch 'ft/bundle-2' that you pushed to was renamed to 'dev'.
remote:
To https://github.com/tnkundwa/Gym-Git-Exercise-Solutions.git
 * [new branch]      HEAD -> ft/bundle-2

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git stash pop
On branch dev
Your branch is up to date with 'origin/ft/bundle-2'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped refs/stash@{0} (c046450615d8e9d87b466d784211628ed71e13d3)

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git stash list

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git reset --hard
HEAD is now at d226dbf This is the home and team

LONOVO@toussaintn23 MSYS ~/Git Exercises (dev)
$ git stash list
```

#Bundle 2
## Exercise 1
```bash
LONOVO@toussaintn23 MSYS ~/Git Exercises (main)
$ git checkout -b "ft/bundle-3"
Switched to a new branch 'ft/bundle-3'

LONOVO@toussaintn23 MSYS ~/Git Exercises (ft/bundle-3)
$ git branch
  dev
* ft/bundle-3
  main

LONOVO@toussaintn23 MSYS ~/Git Exercises (ft/bundle-3)
$ git add services.html 

LONOVO@toussaintn23 MSYS ~/Git Exercises (ft/bundle-3)
$ git commit -m "Working on exercise 3"
[ft/bundle-3 750bd2a] Working on exercise 3
 1 file changed, 11 insertions(+)
 create mode 100644 services.html

LONOVO@toussaintn23 MSYS ~/Git Exercises (ft/bundle-3)
$ git push
fatal: The current branch ft/bundle-3 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-3

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


LONOVO@toussaintn23 MSYS ~/Git Exercises (ft/bundle-3)
$ git push --set-upstream origin ft/bundle-3
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 466 bytes | 233.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/bundle-3' on GitHub by visiting:
remote:      https://github.com/tnkundwa/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-3
remote:
To https://github.com/tnkundwa/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-3 -> ft/bundle-3
branch 'ft/bundle-3' set up to track 'origin/ft/bundle-3'.

LONOVO@toussaintn23 MSYS ~/Git Exercises (ft/bundle-3)
$
```

##Exercise 2
```bash
LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git status
On branch ft/service-redesign
nothing to commit, working tree clean

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git add .

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git commit -m "Added some new services"
[ft/service-redesign 5a38c1e] Added some new services
 1 file changed, 6 insertions(+)

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 370 bytes | 370.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/tnkundwa/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/tnkundwa/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git status
On branch ft/service-redesign
Your branch is up to date with 'origin/ft/service-redesign'.

nothing to commit, working tree clean

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git add .

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git commit -m "Added other new services"
[main 4b301da] Added other new services
 1 file changed, 6 insertions(+)

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 367 bytes | 367.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/tnkundwa/Gym-Git-Exercise-Solutions.git
   dc94141..4b301da  main -> main

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (main)
$ git checkout ft/service-redesign 
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git diff

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git diff main
diff --git a/services.html b/services.html
index 0234b54..f25fce6 100644
--- a/services.html
+++ b/services.html
@@ -9,10 +9,10 @@
     <h1>Our services</h1>
     <h2>We now have a new service!</h2>
     <ol>
-        <li>Service 5</li>
-        <li>Service 6</li>
-        <li>Service 7</li>
-        <li>Service 8</li>
+        <li>Service 1</li>
+        <li>Service 2</li>

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git merge main
-        <li>Service 6</li>
-        <li>Service 7</li>
-        <li>Service 8</li>
+        <li>Service 1</li>
+        <li>Service 2</li>

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git merge main
+        <li>Service 1</li>
+        <li>Service 2</li>

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git merge main

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git merge main
LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git merge main
$ git merge main
Auto-merging services.html
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign|MERGING)
$ git status
On branch ft/service-redesign
Your branch is ahead of 'origin/ft/service-redesign' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git add .

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git commit -m "Combined both services"
On branch ft/service-redesign
Your branch is ahead of 'origin/ft/service-redesign' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 387 bytes | 193.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/tnkundwa/Gym-Git-Exercise-Solutions.git
   5a38c1e..5459e08  ft/service-redesign -> ft/service-redesign

LONOVO@toussaintn23 MINGW64 ~/Git Exercises (ft/service-redesign)
$
```