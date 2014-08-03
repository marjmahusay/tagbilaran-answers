# Setup & Workflow

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
