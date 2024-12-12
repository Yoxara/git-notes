
| **Action**                              | **Command**                                      | **Description**                                                                                   |
|-----------------------------------------|-------------------------------------------------|-----------------------------------------------------------------------------------------------|
| **Clone a repository**                  | `git clone <URL>`                               | Creates a local copy of a remote repository.                                                  |
| **Check status**                        | `git status`                                    | Displays staged, unstaged, and untracked changes.                                             |
| **Stage changes**                       | `git add <file>` / `git add .`                  | Adds changes to the staging area for the next commit.                                         |
| **Commit staged changes**               | `git commit -m "<message>"`                     | Saves changes to the local repository with a message.                                         |
| **Push commits to remote**              | `git push origin <branch>`                      | Uploads local commits to the remote branch.                                                  |
| **Pull updates from remote**            | `git pull origin <branch>`                      | Fetches and merges changes from the remote branch into your current branch.                  |
| **Fetch updates without merging**       | `git fetch`                                     | Downloads changes from the remote without affecting your branch.                             |
| **Merge fetched changes**               | `git merge <remote>/<branch>`                   | Combines changes from the remote branch into your current branch.                            |
| **Reapply commits on top of updates**   | `git rebase <remote>/<branch>`                  | Moves your local commits to the tip of the updated branch, creating a linear history.        |
| **Create a new branch**                 | `git checkout -b <branch-name>`                 | Creates and switches to a new branch for isolated changes.                                   |
| **Switch to an existing branch**        | `git checkout <branch>`                         | Changes to another branch in your repository.                                                |
| **List all branches**                   | `git branch -a`                                 | Shows local and remote branches.                                                             |
| **Delete a local branch**               | `git branch -d <branch>`                        | Deletes a branch locally if it has been merged.                                              |
| **Delete a remote branch**              | `git push origin --delete <branch>`             | Removes a branch from the remote repository.                                                 |
| **View commit history**                 | `git log`                                       | Shows the history of commits for the current branch.                                         |
| **Compact commit history**              | `git log --oneline --graph --all`               | Displays a concise, graphical commit history.                                                |
| **Compare changes between commits**     | `git diff <commit1> <commit2>`                  | Shows differences between two specific commits.                                              |
| **Revert last commit (keep changes)**   | `git reset --soft HEAD~1`                       | Removes the last commit but keeps changes staged.                                            |
| **Revert last commit (discard changes)**| `git reset --hard HEAD~1`                       | Removes the last commit and associated changes.                                              |
| **Unstage a file**                      | `git reset <file>`                              | Removes the file from the staging area.                                                      |
| **Remove untracked files**              | `git clean -f`                                  | Deletes all untracked files from the working directory.                                      |
| **Resolve merge conflicts**             | Edit files manually, then `git add <file>`      | Fix conflicts in files marked with `<<<<<<`, `======`, `>>>>>>`.                             |
| **Continue after resolving conflicts**  | `git merge --continue` / `git rebase --continue`| Completes the merge or rebase process after conflicts are resolved.                          |
| **Abort merge or rebase**               | `git merge --abort` / `git rebase --abort`      | Cancels the merge or rebase process and reverts to the previous state.                       |
| **Push tags to remote**                 | `git push origin <tag-name>`                    | Shares a tag with the remote repository.                                                    |
| **Delete a tag locally**                | `git tag -d <tag-name>`                         | Removes a tag from the local repository.                                                    |
| **Delete a tag remotely**               | `git push origin --delete <tag-name>`           | Removes a tag from the remote repository.                                                   |
| **Create a pull request**               | No command (via GitHub UI)                      | Opens a pull request to merge changes into the target branch.                                |
| **Revert to a specific commit**         | `git reset --hard <commit-hash>`                | Resets the branch to a specific commit and discards later changes.                          |
| **Stash changes**                       | `git stash`                                     | Temporarily saves uncommitted changes and reverts the working directory to a clean state.    |
| **Apply stashed changes**               | `git stash apply`                               | Restores changes from the most recent stash without deleting the stash.                     |
| **Delete a specific stash**             | `git stash drop <stash@{index}>`               | Removes a specific stash from the stash list.                                               |
