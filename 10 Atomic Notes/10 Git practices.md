---
Subjects:
  - git
tags:
  - concept
  - academics
aliases:
  - git
status: WIP
created: 2025-05-20 20:09
updated: 2025-05-20 20:09
---
---
## Overview
Things you should do with your repositories

## classic workflow
`git commit` takes a snapshot of your work in your current branch
`git status` shows you which files are being tracked and what remote you're connected to

**When you have something ready**
1. `git commit`: take a snapshot of your current work, stored locally, and that you don't lose anything on pulling. Also allows you to stage your changes to be pushed
2. `git pull <origin> <branch>`: equivalent of taking all changes in the remote repository (if there are any) and merging them with your current workspace(sorta like `git fetch`and `git merge`)
3. `git push <origin> <branch>`: once you ensure everything is up to date with the remote, push your changes 

 **Merging from a development branch into the main branch**
 1. `git commit`: on your local development branch to take a snapshot, make sure all changes that are tracked are committed else you'll lose your changes on the next step (or use `git stash`)
 2. `git checkout main`: switch to your main branch
 3. `git merge <branch you want to merge into main>`: automatically merges the changes from the local development branch into your main branch
4. Main branch is now up to date with your test branch

---
#### Linked Concepts (Auto-Generated)
```dataviewjs
// Requires Dataview plugin. Lists outgoing links from this note's body
// that likely point to other Atomic Notes (by checking the path).
const outlinks = dv.current().file.outlinks;
// Filter for links pointing to the '10 Atomic Notes' folder (adjust path if needed)
const conceptLinks = outlinks.filter(link => link.path.startsWith("10 Atomic Notes/"));
if (conceptLinks.length > 0) {
    dv.list(conceptLinks);
} else {
    dv.paragraph("No links to other Atomic Notes detected in the body.");
}
```



