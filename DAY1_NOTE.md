### Git: 
+ Git is a software installed locally on the system.
+ Git is maintained by linux.
+ It is a version control system to manage source code history. 

### GitHub
+ GitHub is a service hosted on the web.
+ GitHub is maintained by Microsoft.
+ GitHub is a hosting service for Git repositories.

[Read More](https://www.geeksforgeeks.org/difference-between-git-and-github/
)

📁  A Git repository is the folder.<br /><br />

 ## :fire: **Difference between** <u>Terminal</u>, <u>Console</u>, <u>Shell</u> and <u>Command Line</u><br /><br />
 
### <mark>Terminal</mark> :
- A terminal is a text input and output environment.
- A terminal is a program that allows you to run a shell.
- A terminal is a text input and output environment. 
- A terminal is a wrapper program that runs a shell and allows us to enter commands.

### <mark>Console</mark> :
+ A console is a type of terminal. 
+ Is a window in which your text-mode programs are active. 
+ This window recognizes key presses and is aware of its width and height. 
+ A physical terminal is referred to as a console.

### <mark>Shell</mark> :
- A shell is a program that processes commands and outputs the results. 
- A shell is a layer that sits on top of the kernel: 
- It interprets and processes the commands entered by the user.<br /><br />
Some examples of shells are:<br />
+ Bash
+ Power Shell
+ cmd

### <mark>Command-Line</mark> :
+ This is the line where you type commands.
+ A command-line interface (CLI) is a computer program that processes commands in the form of lines of text. 
The user typically interacts with the shell via a command-line interface (CLI).

[Read More](https://www.geeksforgeeks.org/difference-between-terminal-console-shell-and-command-line/)<br /><br />

### Git CMD :fire: Git Bash  <br /><br />

<u>Git CMD</u>: is just like regular Windows command prompt with the git command. It lets you use all of Git features through command line.<br />
<u>Git Bash</u> is a Unix shell and command language
Git Bash emulates a bash environment on windows.

**
**
<br />

#### 1. <mark>Creating Git Folder</mark><br /><br />
    cd Desktop/
    mkdir Exercises Play

* Now that we are in the correct directory. We can start by initializing Git!

#### 2. <mark>Initialize Git</mark><br /><br />
    git init 

* <u>Note</u>: Git now knows that it should watch the folder you initiated it on.
* Git creates a hidden folder to keep track of changes.

#### 3. <mark>Configure Git</mark><br />
*   Now let Git know who you are. <br />

        git config --global user.name userName
        git config --global user.email userEmail       


#### 4. <mark>Creat Note</mark><br /><br />
    touch day.md
    code day.md
#### 5. <mark>Check The Status</mark><br /><br />
     git status

 * Now Git is aware of the file, but has not added it to our repository!

* Files in your Git repository folder can be in one of 2 states:<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<u>Tracked</u> - files that Git knows about and are added to the repository
<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<u>Untracked</u> - files that are in your working directory, but not added to the repository

* When you first add files to an empty repository, they are all untracked. To get Git to track them, you need to stage them, or add them to the staging environment.

* Staged files are files that are ready to be committed to the repository you are working on. 
So we can add it to the Staging Environment:<br />

        git add .

* Untracked files are files that have been created within your repo's working directory but have not yet been added to the repository's tracking index using the git add command.This is the state of new files you add to your repository. That basically means Git is aware the file exists, but still hasn't saved it in its internal database

#### 6. <mark>Check The Status</mark><br /><br />
     git commit -m 'First time Commit'
* When we commit, we should always include a message.

* By adding clear messages to each commit, it is easy for yourself (and others) to see what has changed and when.

* The commit command performs a commit, and the -m "message" adds a message.

#### 7. <mark>Git Commit Log</mark><br /><br />
     git commit log

* To view the history of commits for a repository, you can use the log command:


#### 8. <mark>Create Repository On GitHub</mark><br /><br />

#### 9. <mark>Add the Repo Link</mark><br /><br />
     git remote add origin url

#### 10. <mark>Push it to GitHub</mark><br /><br />
     git push -u origin master
     

**
**
<br />



### Types of Hacker based on Ethics
+ Black Hat
+ Grey Hat
+ White Hat 

### Types of Hacker based on Skill
+ Newbi/Noob
+ Script Kiddie
+ Hacker
+ Elite/Pro Hacker

### CIA Traid
+ Confidentiality
+ Integrity 
+ Availability 

### Skills:
+ Programming
+ Networking
+ Linux
+ System Admin


### Phase of Hacking
+ Reconnaissance
+ Scanning
+ Gaining Access
+ Maintaing Access
+ Cover Tracks/Clearing Tracks or Logs

### Types of Pen Testing
+ Black Box
+ White Box
+ Grey Box

