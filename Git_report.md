Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~
$ git --version
git version 2.55.0.windows.5

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~
$ cd Desktop
bash: cd: Desktop: No such file or directory

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~
$ git clone https://github.com/alyssalobos/Software-Versioning-Lab.git
Cloning into 'Software-Versioning-Lab'...
remote: Enumerating objects: 14, done.
remote: Counting objects: 100% (14/14), done.
remote: Compressing objects: 100% (11/11), done.
remote: Total 14 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (14/14), done.

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~
$ cd Software-Versioning-Lab

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~/Software-Versioning-Lab (main)
$ ls
Git_report.md  LICENSE  README.md

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~/Software-Versioning-Lab (main)
$ git checkout -b feature-update
Switched to a new branch 'feature-update'

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~/Software-Versioning-Lab (feature-update)
$ code .

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~/Software-Versioning-Lab (feature-update)
$ git status
On branch feature-update
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~/Software-Versioning-Lab (feature-update)
$ git add .

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~/Software-Versioning-Lab (feature-update)
$ git status
On branch feature-update
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md


Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~/Software-Versioning-Lab (feature-update)
$ git commit -m "Update README with laboratory information"
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'Alyssa May@LAPTOP-01V3TTV2.(none)')

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~/Software-Versioning-Lab (feature-update)
$ git config --global user.name "Alyssa Lobos"

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~/Software-Versioning-Lab (feature-update)
$ git config --global user.email "amflobos@mymail.mapua.edu.ph"

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~/Software-Versioning-Lab (feature-update)
$ git config --global user.name
Alyssa Lobos

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~/Software-Versioning-Lab (feature-update)
$ git config --global user.email
amflobos@mymail.mapua.edu.ph

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~/Software-Versioning-Lab (feature-update)
$ git commit -m "Update README with laboratory information"
[feature-update 5675e0b] Update README with laboratory information
 1 file changed, 5 insertions(+), 3 deletions(-)

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~/Software-Versioning-Lab (feature-update)
$ git push origin feature-update
info: please complete authentication in your browser...
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 413 bytes | 413.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'feature-update' on GitHub by visiting:
remote:      https://github.com/alyssalobos/Software-Versioning-Lab/pull/new/feature-update
remote:
To https://github.com/alyssalobos/Software-Versioning-Lab.git
 * [new branch]      feature-update -> feature-update

Alyssa May@LAPTOP-01V3TTV2 MINGW64 ~/Software-Versioning-Lab (feature-update)
$ git push origin feature-update
Everything up-to-date
