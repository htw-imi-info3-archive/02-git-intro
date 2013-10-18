
Demo in Class 17/10/2013
=============================


History first Terminal Window
------------------------------
     mkdir gitdemo
     cd gitdemo/
     mkdir repo1
     cd repo1/
     vi firstfile
     ls
     git init
     ls .git/
     git status
     rm -rf .git/
     ls -lart
     git status
     git init
     git status
     git add firstfile
     git status
     git commit -m "initial version"
     git log
     vi firstfile
     git status
     git commit -am "added a line"
     ls
     git log
     touch a b c
     ls
     git status
     git add .
     git status
     git commit -m "drei neue dateien"
     rm a
     git status
     git add . -u
     git status
     git commit -m "deleted a"
     git rm b
     git status
     git log
     git log --graph
     git log --graph --oneline
     git lg1
     git checkout -b firstbranch
     git lg1
     ls
     git rm c
     git commit -m"deleted file in branch"
     git lg1
     git checkout master
     git lg1
     vi firstfile
     git commit -am "change in master"
     git lg1
     ls
     git status
     git branch
     git checkout firstbranch
     ls
     git checkout master
     git merge firstbranch
     git lg1
     ls
     vi firstfile
     git commit -am "firstfile changed in master"
     git checkout firstbranch
     vi firstfile
     git commit -am "firstfile changed in branch"
     git lg1
     git checkout master
     git merge firstbranch
     ls
     vi firstfile
     git add .
     git commit -m "manually merged firstfile"
     git lg1
     cd .git/
     ls
     cd objects/
     ls
     cd 24
     ls
     cd ..
     cd ..
     ls
     ls -lart
     less HEAD
     ls refs/heads/master
     cat refs/heads/master
     cd ..
     git lg1
     pwd
     git lg1
     git pull ../repo2 cloneb
     ls
     git branch
     less .git/config
     git remote add myclone ../repo2
     less .git/config
     history

History second Terminal Window
------------------------------
     git clone repo1 repo2
     cd repo2
     git checkout -b cloneb
     vi filefromclone
     git add .
     git commit -m "new file in new branch"
     git lg1
     less .git/config
     history
