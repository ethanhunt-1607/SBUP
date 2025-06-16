Hello World !!!!



Microsoft Windows [Version 10.0.22631.3958]
(c) Microsoft Corporation. All rights reserved.

C:\Users\SBUP\MCA2403065>git clone https://github.com/ethanhunt-1607/SBUP.git
Cloning into 'SBUP'...
warning: You appear to have cloned an empty repository.

C:\Users\SBUP\MCA2403065>cd SBUP

C:\Users\SBUP\MCA2403065\SBUP>echo "#MY Git Practice"> README.md

C:\Users\SBUP\MCA2403065\SBUP>git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\SBUP\MCA2403065\SBUP>git add README.md

C:\Users\SBUP\MCA2403065\SBUP>git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md


C:\Users\SBUP\MCA2403065\SBUP>git commit -m "Initial commit on ReadMe file"
[main (root-commit) ce81a1d] Initial commit on ReadMe file
 Committer: unknown <SBUP@UGS-LB4-PC014.sbup.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 README.md

C:\Users\SBUP\MCA2403065\SBUP>git status
On branch main
Your branch is based on 'origin/main', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

nothing to commit, working tree clean

C:\Users\SBUP\MCA2403065\SBUP>git push origin main
info: please complete authentication in your browser...
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 257 bytes | 257.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/ethanhunt-1607/SBUP.git
 * [new branch]      main -> main

C:\Users\SBUP\MCA2403065\SBUP>git branch feature-update

C:\Users\SBUP\MCA2403065\SBUP>git commit
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

C:\Users\SBUP\MCA2403065\SBUP>git switch feature-update
Switched to branch 'feature-update'

C:\Users\SBUP\MCA2403065\SBUP>git add .

C:\Users\SBUP\MCA2403065\SBUP>git commit -m "File updated"
[feature-update 0c864e3] File updated
 Committer: unknown <SBUP@UGS-LB4-PC014.sbup.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)

C:\Users\SBUP\MCA2403065\SBUP>git push origin feature-update
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 290 bytes | 290.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'feature-update' on GitHub by visiting:
remote:      https://github.com/ethanhunt-1607/SBUP/pull/new/feature-update
remote:
To https://github.com/ethanhunt-1607/SBUP.git
 * [new branch]      feature-update -> feature-update

C:\Users\SBUP\MCA2403065\SBUP>git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

C:\Users\SBUP\MCA2403065\SBUP>git merge origin/feature-update
Updating ce81a1d..0c864e3
Fast-forward
 README.md | 1 +
 1 file changed, 1 insertion(+)

C:\Users\SBUP\MCA2403065\SBUP>git push origin main
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/ethanhunt-1607/SBUP.git
   ce81a1d..0c864e3  main -> main

C:\Users\SBUP\MCA2403065\SBUP>git switch feature-update
M       README.md
Switched to branch 'feature-update'

C:\Users\SBUP\MCA2403065\SBUP>git add .

C:\Users\SBUP\MCA2403065\SBUP>git commit -m"Feature updated again"
[feature-update beec5f7] Feature updated again
 Committer: unknown <SBUP@UGS-LB4-PC014.sbup.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+), 1 deletion(-)

C:\Users\SBUP\MCA2403065\SBUP>git push origin feature update
error: src refspec feature does not match any
error: src refspec update does not match any
error: failed to push some refs to 'https://github.com/ethanhunt-1607/SBUP.git'

C:\Users\SBUP\MCA2403065\SBUP>git push origin feature-update
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 293 bytes | 293.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/ethanhunt-1607/SBUP.git
   0c864e3..beec5f7  feature-update -> feature-update

C:\Users\SBUP\MCA2403065\SBUP>git check
git: 'check' is not a git command. See 'git --help'.

The most similar command is
        checkout

C:\Users\SBUP\MCA2403065\SBUP>git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

C:\Users\SBUP\MCA2403065\SBUP>git merge origin/feature-update
Updating 0c864e3..beec5f7
Fast-forward
 README.md | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

C:\Users\SBUP\MCA2403065\SBUP>git push origin main
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/ethanhunt-1607/SBUP.git
   0c864e3..beec5f7  main -> main
