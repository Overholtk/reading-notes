## Revisions and the Cloud

### Version Control
- allows you to see all versions of a file to keep track of updates
- Local VCS: Version control on the computer's hard disk
- CVCS: Version control on a server that all involved parties can access
- allows for easier collaboration between a development team
- DVCS: Data backup
- Allows simultaneous work

### Git
- DVCS
- Stores a snapshot of the file every time you save "commit"
- Primarily uses local operations
- Allows you to work offline
- Three File States:
  - Committed: Stored in local database
  - Modified: Changed, but not stored
  - Staged: Flagged to be changed and stored

### Setting up a Git Repository
- Import:
  - Switch to the proper directory
  - Use the git init command
  - Perform and initial commit
- Cloning:
  - Creates a copy of an existing repository using `"git clone"` with the repository's URL
  - Copies all versions of all files
  - Adding a directory name to the end of the command will clone to a specific directory

## Workflow
- Three Componenets of the local repository:
  - Working Directory: Where the files live
  - Index: Used for staging
  - Head: Most recent Commit
- Tracked vs. Untracked
  - Tracked: can be modified, unmodified, or staged. part of the most recent file snapshot
  - Untracked: not in the last snapshot, do not reside in the staging area
- Check file state using the `git status` command
- Track a single file using `git add FILENAME`
- Track all files in a repository using `git add *`
- Commands track and stage files for committing
- Commit changes in a file and record updates with the `git commit -m "commit message here"` command
- Commit all changes using the `git commit -a` command
- Push changes to the remote repository
  -  ex : `git push origin master`
- `git stash` temporarily hides changes to give a clean working directory
  - use `git stash apply` to retrieve the changes

## Remote Repositories
- the `git remote` command allows you to view the names of remote handles
- using `git remote -v` allows you to view all URLs
