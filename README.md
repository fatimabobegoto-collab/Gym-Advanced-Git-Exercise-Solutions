# Gym-Advanced-Git-Exercise-Solutions

##Bundle 2 exo2 
```bash
applelab@uok-i-mac22 Aziel  GIT % ls -a
.               ..              .git            Git-exercise    git-survival
applelab@uok-i-mac22 Aziel  GIT % git clone https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
Cloning into 'Gym-Advanced-Git-Exercise-Solutions'...
remote: Enumerating objects: 19, done.
remote: Counting objects: 100% (19/19), done.
remote: Compressing objects: 100% (12/12), done.
remote: Total 19 (delta 4), reused 11 (delta 2), pack-reused 0 (from 0)
Receiving objects: 100% (19/19), 4.69 KiB | 4.69 MiB/s, done.
Resolving deltas: 100% (4/4), done.
applelab@uok-i-mac22 Aziel  GIT % ls -a
.                                       Git-exercise
..                                      git-survival
.git                                    Gym-Advanced-Git-Exercise-Solutions
applelab@uok-i-mac22 Aziel  GIT % cd Gym-Advanced-Git-Exercise-Solutions
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % ls -a
.               .git            home.html       README.md       team.html       text2.txt
..              about.html      home.html.save  service.html    text1.txt       text3.txt
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git branch
* main
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git pull
Already up to date.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % ls -a
.               .git            home.html       README.md       team.html       text2.txt
..              about.html      home.html.save  service.html    text1.txt       text3.txt
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % nano service.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git add .
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git commit -m "update B2E2"
[ft/service-redesign 70ae821] update B2E2
 1 file changed, 1 insertion(+)
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push 
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git remote -v
origin  https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git (fetch)
origin  https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git (push)
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origin main
fatal: unable to access 'https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git/': Could not resolve host: github.com
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git branch -M main
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origin main
fatal: unable to access 'https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git/': Failed to connect to github.com port 443 after 19130 ms: Couldn't connect to server
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 273 bytes | 273.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
   826dcdb..70ae821  main -> main
branch 'main' set up to track 'origin/main'.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origin ft/service-redesign
error: src refspec ft/service-redesign does not match any
error: failed to push some refs to 'https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git'
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git branch
* main
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origin ft/service-redesign
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote: 
To https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git branch
* ft/service-redesign
  main
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % nano service.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git add .
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git commit -m "update"
[ft/service-redesign 32a412a] update
 1 file changed, 1 insertion(+), 1 deletion(-)
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 266 bytes | 266.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
   70ae821..32a412a  ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % nano service.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git add .
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git commit -m "update2"
[main c2b2e4a] update2
 1 file changed, 1 deletion(-)
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 263 bytes | 263.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
   70ae821..c2b2e4a  main -> main
branch 'main' set up to track 'origin/main'.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git diff
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git diff main
diff --git a/service.html b/service.html
index 0ea8464..ba7ff6a 100644
--- a/service.html
+++ b/service.html
@@ -8,6 +8,7 @@
 <body>
     <h1>hello everyone. This my services page </h1>
 <p>Hope you are fine </p>
+<p>Good bye</p>
 <p>Bye</p>
 </body>
 </html>
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git merge ft/service-redesign
Auto-merging service.html
CONFLICT (content): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git add .
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git merge ft/service-redesign
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git commit -m "final commit"
[main 88e18c3] final commit
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push 
To https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origon main
fatal: 'origon' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origin main
To https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git reset --soft HEAD~1
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % nano serbice.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % nano service.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git pull origin main --rebase
error: cannot pull with rebase: You have unstaged changes.
error: additionally, your index contains uncommitted changes.
error: please commit or stash them.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git add .
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git commit -m "final commi"
[main 1851157] final commi
 1 file changed, 1 insertion(+), 1 deletion(-)
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origin main 
To https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solut
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % 

```


##Bundle 3 exo1

```bash
applelab@uok-i-mac22 Aziel  GIT % ls -a
.                                       Git-exercise
..                                      git-survival
.git                                    Gym-Advanced-Git-Exercise-Solutions
applelab@uok-i-mac22 Aziel  GIT % cd Gym-Advanced-Git-Exercise-Solutions
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git branch
  ft/service-redesign
* main
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout ft/team-page
error: pathspec 'ft/team-page' did not match any file(s) known to git
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % ls -a
.               about.html      README.md       text1.txt
..              home.html       service.html    text2.txt
.git            home.html.save  team.html       text3.txt
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % touch team2.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % nano team2.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git add .
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git commit -m "initial commit bundle3"
[ft/team-page d446d56] initial commit bundle3
 1 file changed, 1 insertion(+)
 create mode 100644 team2.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origin ft/team-page
Enumerating objects: 18, done.
Counting objects: 100% (18/18), done.
Delta compression using up to 8 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (13/13), 3.39 KiB | 3.39 MiB/s, done.
Total 13 (delta 5), reused 3 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (5/5), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions/pull/new/ft/team-page
remote: 
To https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git log --oneline
d446d56 (HEAD -> ft/team-page, origin/ft/team-page) initial commit bundle3
1851157 (main, ft/contact-page) final commi
c2b2e4a (origin/main, origin/HEAD) update2
70ae821 update B2E2
826dcdb Merge pull request #3 from fatimabobegoto-collab/master
1242260 (origin/master) first commit bundle2
1982bae Merge pull request #2 from fatimabobegoto-collab/master
42b03a8 first commit
1d1874a Merge pull request #1 from fatimabobegoto-collab/master
e84e8a4 first commit
525d2aa Initial commit
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout  ft/contact-page 
Switched to branch 'ft/contact-page'
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git cherry-pick d446d56      
[ft/contact-page 4be37ed] initial commit bundle3
 Date: Tue Jun 23 13:43:56 2026 +0200
 1 file changed, 1 insertion(+)
 create mode 100644 team2.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % nano service.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % nano team2.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git add .
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git commit 
Aborting commit due to empty commit message.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git commit -m "new update"
[ft/contact-page 25b4637] new update
 1 file changed, 2 insertions(+)
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origin ft/contact-page

Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 499 bytes | 499.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions/pull/new/ft/contact-page
remote: 
To https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git branch
* ft/contact-page
  ft/service-redesign
  ft/team-page
  main
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % touch faq.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % nano faq.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git add faq.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git commit -m "faq commit"
[ft/faq-page 527c8db] faq commit
 1 file changed, 1 insertion(+)
 create mode 100644 faq.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origin ft/faq-page
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (9/9), 706 bytes | 706.00 KiB/s, done.
Total 9 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions/pull/new/ft/faq-page
remote: 
To https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git revert d446d56               
CONFLICT (modify/delete): team2.html deleted in parent of d446d56 (initial commit bundle3) and modified in HEAD.  Version HEAD of team2.html left in tree.
error: could not revert d446d56... initial commit bundle3
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % 
```

###Bundle3 exo2

```bash
applelab@uok-i-mac22 Aziel  GIT % ls -a
.                                       Git-exercise
..                                      git-survival
.git                                    Gym-Advanced-Git-Exercise-Solutions
applelab@uok-i-mac22 Aziel  GIT % cd Gym-Advanced-Git-Exercise-Solutions
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git branch
  ft/contact-page
* ft/faq-page
  ft/service-redesign
  ft/team-page
  main
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout -b ft/home-page-redes
ign
Switched to a new branch 'ft/home-page-redesign'
warning: cancelling a revert in progress
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout main
team2.html: needs merge
error: you need to resolve your current index first
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git branch
  ft/contact-page
  ft/faq-page
* ft/home-page-redesign
  ft/service-redesign
  ft/team-page
  main
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout main
team2.html: needs merge
error: you need to resolve your current index first
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git branch
  ft/contact-page
  ft/faq-page
* ft/home-page-redesign
  ft/service-redesign
  ft/team-page
  main
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout main
team2.html: needs merge
error: you need to resolve your current index first
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git add . 
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git commit -m "first commit"
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push           
To https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origin main
To https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push -u origin ft/home-page-re
design
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote: 
To https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git checkout ft/home-page-redesign

Switched to branch 'ft/home-page-redesign'
Your branch is up to date with 'origin/ft/home-page-redesign'.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git rebase main
Current branch ft/home-page-redesign is up to date.
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % nano home.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % ls -a
.               about.html      home.html.save  team.html       text2.txt
..              faq.html        README.md       team2.html      text3.txt
.git            home.html       service.html    text1.txt
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % nano home.html
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git add .
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git commit -m "final commit"
[ft/home-page-redesign ad8104e] final commit
 1 file changed, 1 insertion(+)
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 244 bytes | 244.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/fatimabobegoto-collab/Gym-Advanced-Git-Exercise-Solutions.git
   527c8db..ad8104e  ft/home-page-redesign -> ft/home-page-redesign
applelab@uok-i-mac22 Gym-Advanced-Git-Exercise-Solutions % 
```
#Bumdle 5
```bash
applelab@uok-i-mac22 ~ % git clone https://github.com/fatimabobegoto-collab/git-cafe-exercise.git
Cloning into 'git-cafe-exercise'...
remote: Enumerating objects: 107, done.
remote: Counting objects: 100% (15/15), done.
remote: Compressing objects: 100% (11/11), done.
remote: Total 107 (delta 5), reused 4 (delta 4), pack-reused 92 (from 1)
Receiving objects: 100% (107/107), 1.95 MiB | 574.00 KiB/s, done.
Resolving deltas: 100% (5/5), done.
applelab@uok-i-mac22 ~ % ls
apple.html              Documents               Library                 Pictures
Applications            Downloads               mhealth                 Public
Desktop                 git-cafe-exercise       Movies
Development             index.html              Music
applelab@uok-i-mac22 ~ % cd git-cafe-exercise
applelab@uok-i-mac22 git-cafe-exercise % ls -a
.               bat             index-1.html    index-4.html    README.md
..              css             index-2.html    index.html
.git            images          index-3.html    js
applelab@uok-i-mac22 git-cafe-exercise % nano index.html
applelab@uok-i-mac22 git-cafe-exercise % git add index.htmljm
fatal: pathspec 'index.htmljm' did not match any files
applelab@uok-i-mac22 git-cafe-exercise % git add index.html  
applelab@uok-i-mac22 git-cafe-exercise % git commit -m "correction: place -> restaurant"
[main d209111] correction: place -> restaurant
 1 file changed, 288 insertions(+), 288 deletions(-)
applelab@uok-i-mac22 git-cafe-exercise % git remote -v
origin  https://github.com/fatimabobegoto-collab/git-cafe-exercise.git (fetch)
origin  https://github.com/fatimabobegoto-collab/git-cafe-exercise.git (push)
applelab@uok-i-mac22 git-cafe-exercise % git push    
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.36 KiB | 1.36 MiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/fatimabobegoto-collab/git-cafe-exercise.git
   d1d3f9c..d209111  main -> main
```
