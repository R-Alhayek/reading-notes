# Setting up a Git Repository
**Importing**
To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:

Switch to the target project’s directory
Example:

$ cd test (cd = change directory)
Use the git init command
$ git init
Note: At this stage, you have created a new subdirectory named .git that has the repository files. Tracking has not commenced.

To start tracking these repository files, perform an initial commit by typing the following:
$ git add *.c
$ git add LICENSE
$ git commit -m “any message here”
Now, your files are tracked and there’s an initial commit. We will discuss the particular commands in detail soon.

**Cloning**
You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:

$ git clone https://github.com/test
By cloning the file, you have copied all versions of all files for a project. This command leads to the creation of a directory called “test,” with an initialized .git directory inside it, which has copies of all versions of all files for the specified project. The command also automatically checks out — or retrieves for editing — a copy of the newest version of the project.

To clone a repository into a directory with another name of your choosing, use the following command format:

$ git clone https://github.com/test mydirectory
The command above makes a copy of the target repository in a directory named “mydirectory.”


