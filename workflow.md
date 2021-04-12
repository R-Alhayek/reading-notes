# Workflow
Local Repository Structure
The local Git repository has three components:

Working Directory: The actual files reside here.
Index: The area used for staging
Head: Points to the most recent commit
image03

Saving Changes
All files in a checked out (or working) copy of a project file are either in a tracked or untracked state.

Tracked

Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.

Untracked

Untracked files were not in the last snapshot and do not currently reside in the staging area.

*After cloning a repository, files have tracked status and are unmodified because they have been checked out but not edited.

The Life Cycle of File Status
After you edit a file, Git flags it as modified because of changes made after the previous commit.
You stage the modified file.
Then, you commit staged changes.
image00

Check File Status
To determine the state of files, utilize the git status command:

$ git status
On branch master

nothing to commit, working directory clean

*This information indicates which branch you’re on (we will cover branches in a later section) and states “working directory clean,” which means that files have tracked or modified status at the moment. Also, no untracked files are present because Git has not listed any.

Tracking and Staging a New File
Single File

Track one file only by using the following format:

git add filename
All Files

Track all files in a repository by using the following command:

$ git add *
*After using these commands, files are tracked and staged for committing.

After adding a new file called EXAMPLE, you would see information regarding changes to be committed when using the git status command:

$ git status

On branch master

Changes to be committed:

  (use "git reset HEAD ..." to unstage)
new file: EXAMPLE
This information tells us that there are changes to be committed and that the file has been staged.

Committing a File
After staging one or multiple files, you should commit the changes and record what you did within the commit message:

$ git commit -m “made change x,y,z”
*This step has committed changes for the file or files (you can have one commit message for multiple files, if applicable) to the HEAD.

Committing All Changes
$ git commit -a
*This command commits a snapshot of all modifications to tracked files in the working directory.

Pushing Changes
Next, you would push changes to a remote repository. We will discuss remote repositories in more depth in the next section. For now, we will look at a general overview of pushing changes to remotes.

Example:

$ git push origin master
*This command pushes changes from the local “master” branch to the remote repository named “origin”.

*For cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local repository. However, these names can be changed by the user.