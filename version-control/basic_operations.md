#### Create New Branch And Push :-
* `git checkout -b <branch-name>` :- Creates new branch and checkouts the branch.
* `git push -u origin <branch-name>` :- Pushes branch to the remote and sets the tracking inforamtion.
#### Get Short Hash :- 
* `git log --oneline` :- 
#### Submodules :-
* Submodules allow you to keep a Git repository as a subdirectory of another Git repository. This lets you clone another repository into your project and keep your commits separate.
* To pull a repository with which has submodules use `git pull --recurse-submodules`