# Contributor's Guide

## Setup

1. Make a github account @ https://github.com
2. Download git @ http://git-scm.com and install.
3. In your desktop, click gitbash, in gitbash type:

	```bash
	git config --global user.name "your Firstname your Lastname"
	git config --global user.email youremail@mail.com
	git config --global color.ui auto
	```

4. Fork the main repository @ https://github.com/jangm/tagbilaran-answers.git
5. clone your forked repository in your desired directory, in gitbash type:

	```bash
	git clone "https://github.com/yourusername/tagbilaran-answers.git"
	```

	> After cloning is complete, go to that folder, in gitbash type:

	```bash
	cd tagbilaran-answers
	```
6. Set the upstream to the original repository, in gitbash type:

	```bash
	git remote add upstream https://github.com/jangm/tagbilaran-answers.git
	```

	> If you typed a wrong upstream, in gitbash type:

	```bash
	git remote rm upstream
	```

	> Then set the upstream again correctly.

## Workflow

1. Fetch the files from the main repository, in gitbash type:

	```bash
	git fetch upstream
	```

2. Go to your master branch, in gitbash type:

	```bash
	git checkout master
	```

3. Merge upstream from your forked repository, syncing it, in gitbash type:

	```bash
	git merge upstream/master
	```

4. Make a feature branch, so you could make your own changes or contribution, in gitbash type:

	```bash
	git checkout -b your-feature-example
	```

5. Now you can create your changes, files, folders, etc.

	> Use this commands below in gitbash to monitor your progress.

	```bash
	git status 	# to track files
	git diff 	# to track lines
	git log 	# to user commits
	```

6. Commit those changes to track those changes, in gitbash type:

	```bash
	git commit -am "your description of what you did"
	```

	> You can separate each tasks and commit to that each task for simplicity.

7. You have to push your feature branch in to your forked repository, in gitbash type:

	```bash
	git push origin your-feature-branch
	```

8. After pushing your feature branch into your fork,

	a. Go to your Github account
	b. go to your fork
	c. Select your new feature branch in branch button.
	d. Click the green button at the left to make a pull request
	e. If merge is not able, create comments and discuss conflict
	f. If conflict is resolved or merge is able, click create pull request

9. Wait for the repository integrator to approve the pull request, You'll be notified in your notifications.

10. After the pull request is granted, your contribution has been added to the main repository.
	But your fork is not in sync with the main repository, in gitbash type:

	```bash
	git fetch upstream
	git checkout master
	git merge upstream/master
	git push origin master
	```
11. Your fork is now in sync with the main repository. Repeat steps 1 to 11 in the workflow to contribute.
