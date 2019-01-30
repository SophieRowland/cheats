# Important Git Commands
* Create new repo = `$ git init {new_repo}/`
* Check status of local repo = `$ git status`
* Stage files = `$ git add {new_folder}/{filename}`
* Commit files = `$ git commit -m "Enter commit message here"`
    * `-m` = add message
* Push & set upstream = `$ git push --set-upstream origin master`
    * Push = `$ git push`
    * `origin master` = <remote repo name> <branch name>
* View commit history = `$ git log`
    * To make it look pretty `$ git log --graph --pretty=oneline --abbrev-commit`
* Create new branch = `$ git checkout -b {new_branch}`
* Check status of remote repo = `$ git fetch`
* Update local repo from remote repo = `$ git pull`
    * Specify which remote repo to pull from
* Set another remote repo = '$ git remote add upstream https://github.com/kescobo/git_tutorial.git'
    * "upstream" = repo name
    * https:// = url from clone or download on GitHub
* Pull from remote = `$ git pull`
    * Default pulls from "origin"
    * `$ git pull upstream master`
    * **Double-check** which branch you are on
* Make master branch match dev = `$ git checkout sophdev`
    `$ git merge master`

OR

* Make dev branch match master = `$ git checkout master`
    `$ git merge sophdev`
