

# What is a soft reset?
A soft reset moves the HEAD pointer to an earlier commit while keeping all changes staged. This allows you to recommit the changes without losing your work.

# Comparison Table

Markdown
| Reset Type        | Commit History  | Staging Area         | Working Directory  |        Typical Use Case        |
|-------------------|-----------------|----------------------|--------------------|--------------------------------|
| git reset --soft  | Changes history | Keeps changes staged | Keeps changes      | Redo or combine commits        |
| git reset --mixed | Changes history | Unstages changes     | Keeps changes      | Remove files from staging area |
| git reset --hard  | Changes history | Clears staging area  | Deletes changes    | Completely discard changes     |

# Examples

Soft Reset

Bash
git reset --soft HEAD~1
Expected Result: Last commit removed, changes remain staged.
Mixed Reset

Bash
git reset --mixed HEAD~1
Expected Result: Last commit removed, changes remain in working directory but are unstaged.
Hard Reset
O
Bash
git reset --hard HEAD~1
Expected Result: Last commit and all associated changes are permanently removed.
