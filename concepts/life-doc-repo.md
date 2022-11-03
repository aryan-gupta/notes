This repository is accessed from the [views](/views.md) menu


# Structure
All the files are in `/concept/...` but are sym linked into the other views 
The other views are a combinations of folders and symlinks to items in `/concepts/...`

```
examples:
    /concept/views.md
    /mind/tech/godfile/summary.md -> /concept/godfile-summary.md
    /tech/1/summary.md -> /concept/backup-lvl-1-summary.md
    /security/3/summary.md -> /concept/security-lvl-3-summary.md
    /views.md -> /concept/views.md
```

# Repository
This repository is tracked via git with these special branches:
- main - most items are committed here
- 4 [#public](/security/4/summary.md) data
- 3 [#restricted](/security/3/summary.md) to people I know
- 2 [#confidential](/security/2/summary.md). only friends/family can access upon their discretion
- 1 [#secret](/security/1/summary.md). personal data. friends/family can access upon my discretion

There is a main branch that all items are committed to
There are also 4 branches, one for each data security ring. [details](/security/summary.md)
The main branch is considered #secret as all items will be committed to it
Items get cherry-picked/rebased on to the individual security branches
If something gets committed to a ring branch it will be cherry-picked/rebased onto the main branch
All branches will be pushed to life-doc-private private repository
Only branch 4 (#public) will be pushed to life-doc-public public repository

# Scaling
If we ever need to share more info break into:
life-doc-public becomes life-doc-4
New repo life-doc-3
New repo life-doc-2
life-doc-private becomes life-doc-1
Each repo only has their branch and higher rings
This can be scripted 