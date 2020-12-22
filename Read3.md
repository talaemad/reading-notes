## what is Git?
Distributed Version Control systems ( DVCS ), store data in a way called snapshots, every time you change your project take a snapshot and save it. (the past one and the new) for that, it makes the loss of data few.
the files in git had three states committed, modified, and staged.

## Workflow
Local Repository Structure=> Git repository has three components:
Working Directory: The actual files reside here.
Index: The area used for staging
Head: Points to the most recent commit

## Saving Changes
All files in a checked out (or working) copy of a project file are either in a tracked(can be modified, unmodified, or staged; they were part of the most recent file snapshot.) or untracked state(were not in the last snapshot and do not currently reside in the staging area.).

note: after cloning a repository, files have tracked status and are unmodified because they have been checked out but not edited.


## The Life Cycle of File Status
edit a file => Git flags it as modified => stage the modified file => commit changes.


## Check File Status
 git status command => $ git status
On branch master => nothing to commit, working directory clean

## Tracking and Staging a New File
Single File => git add filename
All Files => $ git add *

note: After using these commands, files are tracked and staged for committing.


## Committing a File
After staging one or multiple files, you should commit the changes => $ git commit -m “made change x,y,z”
note: This step has committed changes for the file or files (you can have one commit message for multiple files, if applicable) to the HEAD.

## Committing All Changes =>$ git commit -a
note: This command commits a snapshot of all modifications to tracked files in the working directory.

## Stashing Changes => git stash
 This command temporarily removes changes and hides them, giving you a clean working directory. When you are ready to continue working on the changes, simply use the git stash apply the command to retrieve the hidden changes.

Remote Repositories =>  You can work with multiple repositories, for which you can have read/write or read-only privileges. Teams can use remote repositories to push information to and pull data from.

Cloned Repositories => for cloned repositories => “origin” to the server from which you cloned and  “master” to your local branch.