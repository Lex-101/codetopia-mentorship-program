
# Restore vs Revert Comparison

|       Command           | Changes Commit History?    | Safe for Shared Repositories?|                                        Typical Use Case                                               |
|-------------------------|----------------------------|------------------------------|-------------------------------------------------------------------------------------------------------|
| git restore             | No                         | Yes                          | Discard uncommitted changes in the working directory and restore files to their last committed state. |
| git restore --staged    | No                         | Yes                          | Remove files from the staging area while keeping the actual file changes intact.                      |
| git revert              | Yes (creates a new commit) | Yes                          | Safely undo a previous commit by creating a new commit that reverses its changes.                     |
| git reset --soft'       | Yes (rewrites history)     | No, use with caution         | Remove recent commits while keeping all changes staged for recommitting.                              |



