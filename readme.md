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