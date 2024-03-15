
| Command                                           | Explanation                                                                                                     |
| ------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| git init                                          | Initializes a new Git repository in the current directory.                                                      |
| git clone \<repository>                           | Clones a repository into a new directory.                                                                       |
| git add \<file>                                   | Adds a file or changes to the staging area.                                                                     |
| git commit -m "\<message>"                        | Commits staged changes with a descriptive message.                                                              |
| git status                                        | Displays the status of the working directory and staging area.                                                  |
| git diff                                          | Shows changes between commits, the index, and the working directory.                                            |
| git log                                           | Displays the commit history.                                                                                    |
| git branch                                        | Lists all local branches in the repository.                                                                     |
| git checkout \<branch>                            | Switches to the specified branch.                                                                               |
| git merge \<branch>                               | Merges changes from the specified branch into the current branch.                                               |
| git pull                                          | Fetches changes from a remote repository and merges them into the current branch.                               |
| git push                                          | Pushes local changes to a remote repository.                                                                    |
| git remote                                        | Lists the remote repositories associated with the current repository.                                           |
| git fetch                                         | Downloads objects and refs from another repository.                                                             |
| git reset \<file>                                 | Unstages changes for a specific file.                                                                           |
| git revert \<commit>                              | Reverts specified commits.                                                                                      |
| git stash                                         | Temporarily saves changes that are not ready to be committed.                                                   |
| git tag \<tagname>                                | Creates a lightweight tag for the current commit.                                                               |
| git rm \<file>                                    | Removes files from the working tree and the index.                                                              |
| git mv \<source> \<target>                        | Moves or renames files, directories, or symlinks.                                                               |
| git show \<object>                                | Shows information about objects like commits, tags, etc.                                                        |
| git config                                        | Sets configuration options for Git.                                                                             |
| git blame \<file>                                 | Shows the author and last modification for each line in a file.                                                 |
| git cherry-pick \<commit>                         | Applies the changes introduced by the specified commit.                                                         |
| git remote add \<name> \<url>                     | Adds a new remote repository with the specified name and URL.                                                   |
| git remote remove \<name>                         | Removes the remote repository with the specified name.                                                          |
| git remote -v                                     | Lists all remote repositories along with their URLs.                                                            |
| git branch -d \<branch>                           | Deletes the specified branch.                                                                                   |
| git branch -m \<new-name>                         | Renames the current branch to the specified new name.                                                           |
| git checkout -b \<branch>                         | Creates a new branch and switches to it.                                                                        |
| git pull \<remote> \<branch>                      | Fetches changes from a remote repository and merges them into the current branch.                               |
| git push \<remote> \<branch>                      | Pushes local changes to the specified remote branch.                                                            |
| git merge --abort                                 | Aborts the current merge operation and resets the index to the state before the merge started.                  |
| git rebase \<branch>                              | Reapplies commits on top of another base tip, typically used to integrate changes from one branch into another. |
| git cherry-pick -n \<commit>                      | Picks a commit from another branch and applies it to the current branch without committing immediately.         |
| git log --graph                                   | Displays the commit history graphically, showing branch and merge history.                                      |
| git submodule add \<url> \<path>                  | Adds a new submodule to the repository at the specified path.                                                   |
| git submodule init                                | Initializes submodules defined in the repository's configuration.                                               |
| git submodule update                              | Updates the registered submodules to their current commit specified in the superproject.                        |
| git clean                                         | Removes untracked files from the working tree.                                                                  |
| git reflog                                        | Shows a log of changes to HEAD (commit history) over time, helpful for recovering lost commits.                 |
| git bisect                                        | Helps to find the commit that introduced a bug by performing a binary search through the commit history.        |
| git log --grep "\<pattern>"                       | Searches the commit history for commits with commit messages matching the specified pattern.                    |
| git archive                                       | Creates a tar or zip archive of the specified tree of files.                                                    |
| git fsck                                          | Verifies the integrity of the Git filesystem.                                                                   |
| ttttttttttttttttttttttttttttttttttttttttttttttttt |                                                                                                                 |
