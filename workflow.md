Workflow
====================

- Make a github account
- https://github.com

- Download git
- http://git-scm.com

- In your desktop, click gitbash, in gitbash type

git config --global user.name "Firstname Lastname"
git config --global user.email youremail@mail.com
git config --global color.ui auto

- In github website, fork the main repository
https://github.com/jangm/tagbilaran-answers.git

- clone your forked repository in your desired directory, in gitbash type
git clone "https://github.com/username/tagbilaran-answers.git"

- set upstream repository to original repository
git remote add upstream https://github.com/jangm/tagbilaran-answers.git

- if wrong upstream, remove upstream by
git remote rm upstream

- fetch files from the main repository to your repository
git fetch upstream

- go to your master branch
git checkout master

- merge remote from your local repository, syncing from the main repository
git merge upstream/master
