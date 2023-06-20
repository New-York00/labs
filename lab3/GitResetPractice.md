# Overview Git reset command

## How

Use git status.
git status - check status

git reset is similar in behavior to git checkout. Where git checkout solely operates on the HEAD ref pointer, git reset will move the HEAD ref pointer and thecurrent branch ref pointer
The default invocation of git reset has implicit arguments of --mixed and HEAD - git reset is equivalent to executing git reset --mixed HEAD

git reset --hard 
The Commit History ref pointers are updated to the specified commit. Then, the Staging Index and Working Directory are reset to match that of the specified commit. Any previously pending changes to the Staging Index and the Working Directory gets reset to match the state of the Commit Tree. This means any pending work that was hanging out in the Staging Index and Working Directory will be lost.

git reset --mixed
The Staging Index is reset to the state of the specified commit. Any changes that have been undone from the Staging Index are moved to the Working Directory. 

git reset --soft
The Staging Index and the Working Directory are left untouched. This behavior can be hard to clearly demonstrate. 
