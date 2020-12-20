# Github-Quick-Commands-List
My own Github-Quick-Commands-List for those who cant remember the Github commands at the last moment :) .

#### Cloning a Repo
| Command | Description |
| ------- | ----------- |
|`git clone URL`| Clone *remote* repo/fork to local machine|

### Version Control Commands:
| Command | Description |
| ------- | ----------- |
|`git add .`| Stage all changes|
|`git commit -m "MESSAGE"`| Commit is stores in local GIT version history.|
|`git push`| Sends committed changes of master branch to *remote* repository.|
|`git reset [file]`<br>git reset site.css| Unstages the file BUT preserves the file contents.|
|`git reset [commit]` <br> git reset 20de7a9c682b131261ba2f45f238e985350e10a1|This command undoes all the commits after the specified commit and preserves the changes locally.|
|`git reset --hard [commit]` | This command discards all history and goes back to the specified commit.|
|`git status`| Lists all the files to be committed|
|`git log`| Lists the version history of the current branch.|

#### Branch Control Commands
| Command | Description |
| ------- | ----------- |
|`git branch`| Lists all the local branches in the current repository.|
|`git branch -a`| Lists all branches Local+*remote*|
|`git branch [NEW_NAME]`| Creates **new** branch in the repository with name = NEW_NAME |
|`git branch -d [BRANCH_NAME]`| **Deletes** the specified branch locally.|
|`git branch -m [old branch name] [new branch name]`|Renames a local branch name.|
|`git checkout [NAME]`| Check out from one branch to another.|
|`git checkout -b [NEW_NAME]`| Create a **new** branch and also switches to it.|
|`git remote add [variable name] [remote Server Link]`<br> git remote add origin https://github.com/ojhalakshya/Github-Quick-Commands-List.git|This command is used to connect your local repository to the *remote* server.|

#### GIT MERGE
| Command | Description |
| ------- | ----------- |
|`git merge [BRANCH_NAME]`|To merge a different branch into your active branch.|
|`git merge [source branch] [target branch]`|Merge a branch into target branch|


#### REWRITING HISTORY

| Command | Description |
| ------- | ----------- |
|`git commit --amend`|Modify the Head commit or the most *recent* commit. Allows to combine currently staged changes with the most recent commit.|
|`git commit --amend -m "NEW_MESSAGE"`|Modify the most *recent* commit message.|
|`git rebase -i HEAD~3`<br>pick f7f3f6d commit no 1<br>edit 310154e commit no 2<br>pick a5f4a0d commit no 3|Show commit in the range HEAD ~ 3.<br> To **EDIT** any commit replace pick -> edit, on which the terminal will stop to allow any ammends on it. <br>Afterwards use `git rebase --continue` to allow all other commits.<br> At last use `git push --force`. [Re-Writing History](https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History)|
|`git revert HEAD`|Reverts the changes in previous commit w/o touching it and commits the opposite of the changes in a new commit.|

#### GIT PUSH

| Command | Description |
| ------- | ----------- |
|`git push -u origin feature_branch_name`<br> `git push --set-upstream origin feature_branch_name`|Push **newly** created feature branch to `[variable name] = origin`|
|`git push [variable name] master`|Pushes the changes of the master branch to repository saved by the [variable name]|
|`git push [variable name] [branch]`|Pushes the changes of the specified branch to repository saved by the [variable name]|
|`git push –all [variable name]`|Pushes all the branches to the *remote* repository|
|`git push <remote_name> --delete <branch_name>` <br>OR<br>`git push [variable name] :[branch name]`|These commands **Delete** a branch on your *remote* repository.|

#### GIT PULL

| Command | Description |
| ------- | ----------- |
|`git pull`|Fetch and merge changes on the *remote* server to your working directory.|
|`git pull origin [Repository Link]`|Pulls changes from remote repo to `[variable name] = origin`|


#### GIT FETCH
| Command | Description |
| ------- | ----------- |
|`git fetch <*remote*>`|Fetch all of the branches from the repository. This also downloads all of the required commits and files from the other repository.|
|`git fetch <*remote*> <branch>`|Same as the above command, but only fetch the specified branch.|
|`git fetch --all`|A power move which fetches all registered *remote*s and their branches.|
|`git fetch origin`<br>`git reset --hard origin/master`|Instead, to drop all your local changes and commits, fetch the latest history from the server and point your local master branch at it, do this.|
