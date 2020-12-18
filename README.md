# Github-Quick-Commands-List
My own Github-Quick-Commands-List for those who cant remember the Github commands at the last moment :) .


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
|`git checkout [NAME]`| Check out from one branch to another.|
|`git checkout -b [NEW_NAME]`| Create a **new** branch and also switches to it.|
|`git merge [BRANCH_NAME]`|To merge a different branch into your active branch:|
|`git *remote* add [variable name] [*remote* Server Link]`<br> git *remote* add origin https://github.com/ojhalakshya/Github-Quick-Commands-List.git|This command is used to connect your local repository to the *remote* server.|


#### GIT PUSH

| Command | Description |
| ------- | ----------- |
|`git push -u origin feature_branch_name`|Push **newly** created feature branch to `[variable name] = origin`|
|`git push [variable name] master`|Pushes the changes of the master branch to repository saved by the [variable name]|
|`git push [variable name] [branch]`|Pushes the changes of the specified branch to repository saved by the [variable name]|
|`git push –all [variable name]`|Pushes all the branches to the *remote* repository|
|`git push <*remote*_name> --**Delete** <branch_name>` <br>OR<br>`git push [variable name] :[branch name]`|These commands **Delete** a branch on your *remote* repository.|

#### GIT PULL

| Command | Description |
| ------- | ----------- |
|`git pull`|Fetch and merge changes on the *remote* server to your working directory.|
|`git pull [Repository Link]`|This command fetches and merges changes on the *remote* server to your working directory.|


| Command | Description |
| ------- | ----------- |
|`git fetch <*remote*>`|Fetch all of the branches from the repository. This also downloads all of the required commits and files from the other repository.|
|`git fetch <*remote*> <branch>`|Same as the above command, but only fetch the specified branch.|
|`git fetch --all`|A power move which fetches all registered *remote*s and their branches.|
|`git fetch origin`<br>`git reset --hard origin/master`|Instead, to drop all your local changes and commits, fetch the latest history from the server and point your local master branch at it, do this.|
