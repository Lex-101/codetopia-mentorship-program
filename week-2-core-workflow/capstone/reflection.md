
# When should you use git restore?
Use git restore when you want to discard uncommitted changes in your working directory.

# When should you use git restore --staged?
Use it when a file was accidentally added to the staging area and you want to unstage it.

# Why is git revert safer than rewriting history?
Git revert creates a new commit that undoes changes without altering existing commit history, making it safe for shared repositories.

# What is the difference between revert and reset?
Git revert creates a new commit that undoes previous changes, while git reset moves the branch pointer and can rewrite history.

# What mistake did you make and how did you recover?
I accidentally staged and committed unwanted changes. I used git restore, git restore --staged, and git revert to undo the mistakes safely.

# What did you learn during Week 2?
I learned how Git tracks changes, how to undo mistakes using restore, revert, and reset, and when each command is appropriate.
