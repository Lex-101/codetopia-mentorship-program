
# Mistake 1: Added wrong content
Command:
Bash
echo "It's very fantastic." >> experiment.md
Problem: Accidentally added unwanted content to the file.
Recovery:
	Bash
	git restore restore.md
Result: The file was restored to the last committed version and the incorrect content was removed.

# Mistake 2: Wrong staging
Command:
Bash
git add experiment.md

Problem: Accidentally staged a file that was not ready to be committed.
Recovery:
	Bash
	git restore --staged restore.md
Result: The file was removed from the staging area while keeping the changes in the working directory.

# Mistake 3: Wrong commit message
Commands:
Bash
git add experiment.md
git commit -m "bad commit"

Problem: Used an unclear commit message.
Recovery:
	Bash
	git commit --amend -m "docs: update experiment notes"
Result: The previous commit message was replaced with a more meaningful one.

# Mistake 4: Unwanted commit
Command:
Bash
git commit -m "temporary changes"

Problem: Created a commit that should not have been added to project history.
Recovery:
	Bash
	git reset --soft HEAD~1
Result: The commit was removed from history, but the changes remained staged for further editing.

#Mistake 5: Reverting a commit
Command:
	Bash
	git revert 781bb68
Problem: Needed to undo a commit without rewriting project history.
Result: Git created a new commit that reversed the changes from the selected commit.

#Reflection
This exercise helped me understand the difference between modifying files, staging changes, and committing changes. 
I learned that Git provides different recovery tools depending on whether the mistake is in the working directory, staging area, or commit history.
