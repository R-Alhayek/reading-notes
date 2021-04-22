# Choosing A Text Editor
## What is a text editor?
#### The text editor has to be one of the most important tools you can use as an aspiring web developer. A text editor is a piece of software that you download and install on your computer, or you access online through your web browser, that allows you to write and manage text, especially the text that you write to build a web site.

## Features to look for in a text editor:
1. **Code completion**: Code completion allows you to start typing, and the code completion feature will display possible suggestions based on what you originally typed. This saves you time by providing a choice, rather than allowing you to finish typing and possibly encounter typos.
2. **Syntax highlighting**: Syntax highlighting is a feature that takes the text you type, and makes it more noticeable by colorizing the text. Attributes are a different color than elements. And elements are a different color than copy. This makes it so much easier when you’re looking for an error and you can’t find it. As well as making your text easier to read.
3. **A nice variety of themes**: These themes will allow you to change the color of the background of your text editor, the series of colors in your text, and sometimes themes will affect other aspects of your text editing software as well. Since you’ll be using your text editor most of the time, it’s good to find a theme that might reduce eye strain and fatigue.
4. **Extensions**: A text editor that has a great selection
of extension will ensure that you have the ability to add functionality as you need it.

## Third-Party Options of editors:
+ **NotePad++**: NotePad++ is a free text editor for Windows Computers only. It has syntax highlighting and code completion, as well as word completion and function completion. It has a zoom in an out feature, it’s own online community, and its own chat room for questions that may arise. It even has its own searchable wiki page for more assistance.
+ **Visual Studio Code**: Visual Studio Code is a free text editor.It is available for Windows computers, Mac computers and Linux computers. VS Code has the Emmet shorthand for HTML and CSS already built-in with no additional work from you at all. VS Code has everything: syntax highlighting, themes, extensions and code completion. It seems like VS Code has a very healthy following in the
web developing community.
+ **Atom**: Atom is a free text editor that’s available for download for Windows computers, Mac computers and Linux computers. Atom is brought to you by the folks at GitHub. You can host and review code, or you can post and get help with the development of your own projects. Atom also ticks all the right boxes. It has syntax highlighting, themes, extensions, the works!
![image](https://geekboots.sfo2.cdn.digitaloceanspaces.com/post/code-editor-for-web-developer-1570698798393.jpg)

## The Difference Between Text Editors and IDEs:
#### A text editor kind of gives away what it does in the title—it edits text. It also manages text, and manages files. It wrangles your text together into something meaningful. An IDE (Integrated Development Environment) is really a suite of different software all coming together. An IDE is a text editor, a file manager, a compiler, and a debugger all in one software package.

# The Command Line!
#### A command line, or terminal, is a text based interface to the system. You are able to enter commands by typing them on the keyboard and feedback will be given to you similarly as text. The command line typically presents you with a prompt. As you type, it will be displayed after the prompt. Most of the time you will be issuing commands. 

# Opening a Terminal:
+ If you're on a Mac then you'll find the program Terminal under Applications -> Utilities. An easy way to get to it is the key combination 'command + space' which will bring up Spotlight, then start typing Terminal and it will soon show up.
+ If on Linux then you will probably find it in Applications -> System or Applications -> Utilities. Alternatively you may be able to 'right-click' on the desktop and there may be an option 'Open in terminal'.
+ If you are on Windows and intend to remotely log into another machine then you will need an SSH client. A rather good one is Putty (free) .

# The Shell, Bash:
#### Within a terminal you have what is known as a shell. This is a part of the operating system that defines how the terminal will behave and looks after running (or executing) commands for you. There are various shells available but the most common one is called bash which stands for Bourne again shell.

# Shortcuts:
####  Linux is full of shortcuts to help make your life easier.They make your life easier, they often also save you from making silly mistakes such as typos.
![image](https://www.windowscentral.com/sites/wpcentral.com/files/styles/small/public/field/image/2020/05/terminal-icon.jpg)


# Basic Navigation!
####  In this section, we'll learn the basics of moving around the system. Many tasks rely on being able to get to, or reference the correct location in the system. As such, this stuff really forms the foundation of being able to work effectively in Linux. 
1. **So where are we?**: The first command we are going to learn is **pwd** which stands for Print Working Directory. The command does just that. It tells you what your current or present working directory is. 
2. **What's in Our Current Location?**: It's one thing to know where we are. Next we'll want to know what is there. The command for this task is ls. It's short for list. Whereas pwd is just run by itself with no arguments, ls is a little more powerful. 
3. **Paths**: Whenever we refer to either a file or directory on the command line, we are in fact referring to a path. ie. A path is a means to get to a particular file or directory on the system.
+ **Absolute and Relative Paths**: There are 2 types of paths we can use, absolute and relative. Whenever we refer to a file or directory we are using one of these paths. Whenever we refer to a file or directory, we can, in fact, use either type of path.
   + **Absolute paths** specify a location (file or directory) in relation to the root directory. You can identify them easily as they always begin with a forward slash ( / )
   + **Relative paths** specify a location (file or directory) in relation to where we currently are in the system. They will not begin with a slash.
4. **Let's Move Around a Bit**: In order to move around in the system we use a command called cd which stands for change directory. It works as follows: cd [location]

![image](https://www.howtoforge.com/images/linux_cd_command/big/cd-basic.png)

# About Files!
#### in LENUX, everything is actually a file. A text file is a file, a directory is a file, your keyboard is a file, your monitor is a file, To begin with, this won't affect what we do too much but keep it in mind as it helps with understanding the behaviour of Linux as we manage files and directories.
+ **Linux is an Extensionless System**: A file extension is normally a set of 2 - 4 characters after a full stop at the end of a file, which denotes what type of file it is. The following are common extensions:
    + file.exe - an executable file, or program.
    + file.txt - a plain text file.
    + file.png, file.gif, file.jpg - an image. 
+ **Linux is Case Sensitive**: Other systems such as Windows are case insensitive when it comes to referring to files. Linux is not like this. As such it is possible to have two or more files and directories with the same name but letters of different case. Also be aware of case sensitivity when dealing with command line options.
+ **Spaces in names**: Spaces in file and directory names are perfectly valid but we need to be a little careful with them. As you would remember, a space on the command line is how we seperate items. They are how we know what is the program name and can identify each command line argument.To get around this we need to identify to the terminal that we wish to be seen as a single command line argument. There are two ways to go about this, either way is just as valid.
  + **Quotes**: The first approach involves using quotes around the entire item. You may use either single or double quotes.Anything inside quotes is considered a single item.
  + **Escape Characters**: Another method is to use what is called an escape character, which is a backslash ( \ ). What the backslash does is escape (or nullify) the special meaning of the next character.

+ **Hidden Files and Directories**: Linux actually has a very simple and elegant mechanism for specifying that a file or directory is hidden. If the file or directory's name begins with a . (full stop) then it is considered to be hidden. You don't even need a special command or action to make a file hidden.
  + To make a file or directory hidden all you need to do is create the file or directory with it's name beginning with a . or rename it to be as such. Likewise you may rename a hidden file to remove the . and it will become unhidden. The command ls which we have seen in the previous section will not list hidden files and directories by default. We may modify it by including the command line option -a so that it does show hidden files and directories.

![image](https://icons.iconarchive.com/icons/saki/nuoveXT/128/Folder-linux-icon.png)

