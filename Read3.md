<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>Revisions and the Cloud</title>
  </head>
  <body style="background-color: darkslategray; color: hotpink;">
    <header>
    </header>
    <main>
	<p>
		
what is Git?
		<br>

Distributed Version Control systems ( DVCS ), store data in a way called snapshots, every time you change your project take a snapshot and save it. (the past one and the new) for that, it makes the loss of data few.
the files in git had three states committed, modified, and staged.
<br>
Workflow
		<br>

Local Repository Structure=> Git repository has three components:
		<br>

Working Directory: The actual files reside here.

		<br>
Index: The area used for staging

		<br>
Head: Points to the most recent commit
<br>

Saving Changes

		<br>
All files in a checked out (or working) copy of a project file are either in a tracked(can be modified, unmodified, or staged; they were part of the most recent file snapshot.) or untracked state(were not in the last snapshot and do not currently reside in the staging area.).
<br>

note: after cloning a repository, files have tracked status and are unmodified because they have been checked out but not edited.
<br>



		
	The Life Cycle of File Status
<br>

		edit a file => Git flags it as modified => stage the modified file => commit changes.


Check File Status
		<br>

git status command => $ git status
		<br>

On branch master => nothing to commit, working directory clean
<br>

Tracking and Staging a New File
		<br>

Single File => git add filename
		<br>

All Files => $ git add *
<br>

note: After using these commands, files are tracked and staged for committing.

<br>

Committing a File
		<br>

After staging one or multiple files, you should commit the changes => $ git commit -m “made change x,y,z”
		<br>

note: This step has committed changes for the file or files (you can have one commit message for multiple files, if applicable) to the HEAD.
<br>

Committing All Changes =>$ git commit -a
		<br>

note: This command commits a snapshot of all modifications to tracked files in the working directory.
<br>

Stashing Changes => git stash
<br>

		This command temporarily removes changes and hides them, giving you a clean working directory. When you are ready to continue working on the changes, simply use the git stash apply the command to retrieve the hidden changes.
<br>

Remote Repositories => You can work with multiple repositories, for which you can have read/write or read-only privileges. Teams can use remote repositories to push information to and pull data from.
<br>

Cloned Repositories => for cloned repositories => “origin” to the server from which you cloned and “master” to your local branch.
	</p>
        
    </main>
    <footer>
     	<p>
             Tala Emad
        </p>
    </footer>
  </body>
</html>
