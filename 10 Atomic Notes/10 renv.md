---
Subjects:
  - R
tags:
  - academics
  - guide
aliases:
  - r environment
  - renv
status: WIP
created: 2025-05-23 12:08
updated: 2025-05-23 12:08
---
---
## Overview
In this document we will be going through renv, a package that can be used to ensure the portability of R projects across different machines, by ensuring fixed dependencies (and a fixed R environment)

![[Pasted image 20250523121517.png]]


## Commands and Files

remember to tag `renv::` before each of these commands

### 1. Starting up
`init()`: initialises a project library in the root directory of your R.proj file and creates a **lockfile**
	- Run this on a new R proj if you haven't yet
	- This is akin to taking your initial snapshot and storing it

**lockfile**, aka `renv.lock`: a file that stores all the packages currently used in your project and the metadata needed to reinstall the packages currently loaded. (note not the installation of the packages themselves but rather just a list, think of it as a packing list for R)
	- this is what `snapshot` writes to and what `restore` restores from.

`.Rprofile`: a file that is sourced by R, part of every R project (but there also exists a global .Rprofile), every time it starts up, this is not part of renv but rather from base R.
- in the context of `renv`, it tells the current R project which library to look in for its packages
- and this will be the library within the renv file

#### The `renv` folder
- Where your R packages are installed  
	- but this isn't ported over to other computers, as it'll get to big. They rely on the **lockfile** instead
- Where your project specific settings for renv are stored
- Usually has a separate .gitignore file from the rest of the system

### 2. Keeping `renv` up to date as your work
`snapshot`: run this every time you make a change to your dependencies/installations.
- e.g. after you've updated R or your packages, installed new packages 
- You will be notified by a message that says `This project is out of sync` when your renv **lockfile** doesn't match your project library.
- Basically stores a snapshot of your current environment and dependencies

`status`: run this to check how what's in sync/out of sync

### 3. Using renv to load dependencies
`restore`: use this when you have just imported someone else's project and you want to load their dependencies
- installs all packages and R versions according to the **lockfile** 
- This is what others use when loading your renv too






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



