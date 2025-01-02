# Portfolio Repository

## Deskripsi
Repository ini menunjukkan pengalaman saya menggunakan Git dan GitHub, termasuk:
- Membuat folder dan branch repository.
- Mengelola riwayat kodingan.
- Menggunakan Git untuk manajemen kode versi.

## Struktur Repository
- **Main branch**: Berisi kode utama.
- **Feature branches**: Branch terpisah untuk pengembangan fitur baru --> saya namakan: branch_baru.
- **Bugfix branches**: Branch untuk perbaikan bug --> rencana ke depannya.

## Riwayat Pengembangan
1. Membuat repository lokal --> kodingan terlampir.
2. Menambahkan branch `branch_baru` untuk fitur A.
3. Mengintegrasikan perubahan ke branch `main`.

## Teknologi yang Digunakan
- Git
- GitHub

## Riwayat kodingan:
lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git init
Reinitialized existing Git repository in D:/Automate/Edugit/.git/

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ ls -a
./  ../  .git/

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ ^[[200~git remote add origin https://github.com/rahmileejiyoo/LearnGit_CreateRepository.git~
bash: $'\E[200~git': command not found

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ ^C

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git remote add origin https://github.com/rahmileejiyoo/LearnGit_CreateRepository.git
error: remote origin already exists.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ nano file1.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ nano file1.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ nano file1.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git add file1.txt
warning: in the working copy of 'file1.txt', LF will be replaced by CRLF the next time Git touches it

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ ^C

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git add --renormalize file1.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   file1.txt


lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git commit -m "upload new file"
[master (root-commit) e7109b4] upload new file
 Committer: Lia Rahmi Adriani <lia.rahmi@biofarma.co.id>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 file1.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ ^C

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git config --global user.name "rahmileejiyoo"

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git config --global user.email "lrahmiadriani@gmail.com"

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git commit --amend --reset-author
[master dd58d94] upload new file
 1 file changed, 1 insertion(+)
 create mode 100644 file1.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git config --global --list
user.name=rahmileejiyoo
user.email=lrahmiadriani@gmail.com

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git push --force
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ ^C

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git push --set-upstream origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 235 bytes | 235.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/rahmileejiyoo/LearnGit.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git remote -v
origin  https://github.com/rahmileejiyoo/LearnGit.git (fetch)
origin  https://github.com/rahmileejiyoo/LearnGit.git (push)

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ ^C

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git remote add new-origin https://github.com/rahmileejiyoo/LearnGit_CreateRepositoy.git

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git push new-origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 235 bytes | 235.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/rahmileejiyoo/LearnGit_CreateRepository.git
 * [new branch]      master -> master

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git commit --amend --reset-author
[master 44a6b56] upload new file
 1 file changed, 1 insertion(+)
 create mode 100644 file1.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git push --force
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 236 bytes | 236.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/rahmileejiyoo/LearnGit.git
 + dd58d94...44a6b56 master -> master (forced update)

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git remote -v
new-origin      https://github.com/rahmileejiyoo/LearnGit_CreateRepository.git (fetc)
new-origin      https://github.com/rahmileejiyoo/LearnGit_CreateRepository.git (push
origin  https://github.com/rahmileejiyoo/LearnGit.git (fetch)
origin  https://github.com/rahmileejiyoo/LearnGit.git (push)

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ ^C

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git push new-origin master --force
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 236 bytes | 236.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/rahmileejiyoo/LearnGit_CreateRepository.git
 + dd58d94...44a6b56 master -> master (forced update)

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git remote remove origin

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git remote rename new-origin origin
Renaming remote references: 100% (1/1), done.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git remote -v
origin  https://github.com/rahmileejiyoo/LearnGit_CreateRepository.git (fetch)
origin  https://github.com/rahmileejiyoo/LearnGit_CreateRepository.git (push)

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git status
On branch master
nothing to commit, working tree clean

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/rahmileejiyoo/LearnGit_Createepository.git'

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/rahmileejiyoo/LearnGit_Createry.git'

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ ^C

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (master)
$ git branch -m master main

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git push -u origin main
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'main' on GitHub by visiting:
remote:      https://github.com/rahmileejiyoo/LearnGit_CreateRepository/pull/new/mai
remote:
To https://github.com/rahmileejiyoo/LearnGit_CreateRepository.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git checkout -b branch_baru
Switched to a new branch 'branch_baru'

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ nano file2.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ git add file2.txt
warning: in the working copy of 'file2.txt', LF will be replaced by CRLF the next tiouches it

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ git add --renormalize file2.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ git status
On branch branch_baru
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   file2.txt


lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ git commit -m "upload new file"
[branch_baru d8ab9be] upload new file
 1 file changed, 1 insertion(+)
 create mode 100644 file2.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ ls
file1.txt  file2.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ git push branch_baru
fatal: 'branch_baru' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ git push origin branch_baru
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 288 bytes | 288.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'branch_baru' on GitHub by visiting:
remote:      https://github.com/rahmileejiyoo/LearnGit_CreateRepository/pull/new/bra
remote:
To https://github.com/rahmileejiyoo/LearnGit_CreateRepository.git
 * [new branch]      branch_baru -> branch_baru

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ ls
file1.txt  file2.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ git add .

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ git commit -m "added new file"
On branch branch_baru
nothing to commit, working tree clean

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git checkout branch_baru
Switched to branch 'branch_baru'

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git merge branch_baru
Updating 44a6b56..d8ab9be
Fast-forward
 file2.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 file2.txt

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git checkout branch_baru
Switched to branch 'branch_baru'

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git branch
  branch_baru
* main

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git branch -d branch_baru
Deleted branch branch_baru (was d8ab9be).

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git branch
* main

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git pull
Already up to date.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git push
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/rahmileejiyoo/LearnGit_CreateRepository.git
   44a6b56..d8ab9be  main -> main

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git checkout branch_baru
Switched to a new branch 'branch_baru'
branch 'branch_baru' set up to track 'origin/branch_baru'.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ git pull
Already up to date.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (branch_baru)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git branch
  branch_baru
* main

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ ^C

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git branch -d branch_baru
Deleted branch branch_baru (was d8ab9be).

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git push origin --delete branch_baru
To https://github.com/rahmileejiyoo/LearnGit_CreateRepository.git
 - [deleted]         branch_baru

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git add .

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git commit -m "Save all changes"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git push origin main
Everything up-to-date

lia.rahmi@NBSS-D-0599 MINGW64 /d/Automate/Edugit (main)
$ git clone https://github.com/rahmileejiyoo/LearnGit_CreateRepository.git
Cloning into 'LearnGit_CreateRepository'...
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 9 (delta 0), reused 6 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (9/9), done.


