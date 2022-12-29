### Contents
* [Branch Operations](#revert-changes-to-a-specific-commit)
* [Logging Operations](#ogging)
* [Stashing Changes Temporarily](#stashing-changes-temporarily)
* [Submodules](#submodules)
* [Reverting Changes](#reverting-changes)

----------------------------------------

#### Branch Operations :
* `git checkout -b <branch-name>` :- Creates new branch and checkouts the branch.
* `git push -u origin <branch-name>` :- Pushes branch to the remote and sets the tracking information.
#### Logging :
* `git log --oneline` :- to list one commit per line
#### Stashing changes temporarily :
* If one has made changes in a branch then he can't checkout other branches or take pull from the remote. To do so he has commit the changes.
* Stashing is a concept in git in which we can store changes temporarily and the changes those are saved away with `git stash` command would be reverted from the working branch. After this point one can switch branch, take pull from remote and perform other git operations.
* `git stash push -- path/to/folder_or_file` :- stash changes in a directory or a file
* `git stash apply` :- to apply the changes but keeps the changes in stash list
* `git stash pop` :- to apply the changes and delete the changes from the stash list
#### Submodules :
* Submodules allow you to keep a Git repository as a subdirectory of another Git repository. This lets you clone another repository into your project and keep your commits separate.
* To pull a repository with which has submodules use `git pull --recurse-submodules`
#### Reverting Changes :
* To revert changes done in a single file/directory use `git checkout -- path/to/file_or_directory`(doesn't remove untracked files only changes in tracked files)
* To remove all untracked files use `git clean -f`