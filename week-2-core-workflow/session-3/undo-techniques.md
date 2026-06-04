          undo-techniques.md                               Modified
1. git restore
Purpose
Restores a file in the working directory to its last committed state, discarding uncommitted changes.

When to use it:
When you have modified a file and want to remove those changes.

Example command
Bash
git restore restore.md

Expected result
Any uncommitted changes in README.md are removed, and the file matches the latest commit.
Screenshot: Save a screenshot showing the command and result in the screenshots/ folder.

2. git restore --staged
Purpose
Removes a file from the staging area while keeping the changes in the working directory.

When to use it:
When you accidentally staged a file using git add.

Example command
Bash
git restore --staged restore.md

Expected result
The file is no longer staged, but your edits remain in the file.
Screenshot: Save a screenshot showing git status before and after running the command.

3. git revert
Purpose
Creates a new commit that reverses the changes made by a previous commit.

When to use it:
When you need to undo a commit that has already been shared or pushed.

Example command
Bash
git revert HEAD

Expected result
A new commit is created that cancels the changes from the most recent commit.
Screenshot: Save a screenshot of the commit history before and after the revert.

4. git reset --soft
Purpose
Moves HEAD to a previous commit while keeping all changes staged.

When to use it:
When you want to redo or combine commits without losing your work.

Example command
Bash
git reset --soft HEAD~1

Expected result
The last commit is removed from history, but its changes remain staged and ready to commit again.
Screenshot: Save a screenshot showing git log before and after the reset, plus git status.

