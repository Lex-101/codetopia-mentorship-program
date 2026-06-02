The 3 Git states, in simple terms:

Working directory(Modified) – You changed a file, but Git has not marked it for the next commit yet.

Staging area(index) – You selected the changes to be included in the next commit (git add).

RepositoryCommitted(.git folder) – The changes have been permanently saved to the repository's history (git commit).

Flow: Modified → Staged → Committed.

GUI is easier for beginners because it uses visual menus and buttons.
CLI is more useful for advanced users because it is faster and provides greater control through commands.



Git installation verification: git --version

Git configuration commands: 
- git config --global user.name "youname"
- git config --global user.email "your email"

Git commands learned during Week 1
- git init
- git add                       
- git commit -m "commit-message"
- git commit --amend -m ""(only works on recent commit messages)
- git log, git log --oneline, git log --oneline --graph, git log --oneline --all --graph
- git diff --staged(views changes made in the recents commit messages)
