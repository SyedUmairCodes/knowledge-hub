What is Version Control? Version control is a system that tracks changes to files over time, allowing users to revert to previous versions, collaborate effectively, and keep records of who made which changes and why1. Version control systems like Git are more sophisticated than simple track changes features, since they can meticulously track changes on many files with multiple people working simultaneously1. Without version control, users may keep multiple similar copies of files, which can lead to errors and confusion1.

●

Benefits of Version Control: The benefits of version control include keeping a single updated version of each file with a record of all previous versions and a record of exactly what changed between versions1. It helps when collaborating with others by tracking who, when, and why specific changes were made1. It also helps when developing code, since if a mistake is introduced, the user can revert to the original, unbroken code2. Additionally, it allows multiple people to work on the same file and merge all edits into one cohesive file2.

●

Git: Git is a free and open-source version control system that is the most commonly used today2. Git keeps a local copy of your work and revisions that you can use offline. Once the user has internet access, they can sync their local copy with the main online repository2. Git also allows multiple collaborators to work on their own parts of the code simultaneously2. RStudio and Git interface easily with each other2.

●

GitHub: GitHub is an online interface for Git, acting as a host for files and records of changes23. It is similar to Dropbox in that files are both on the user's computer and hosted online34. GitHub allows users to keep repositories private or public, and it interfaces with Git to keep track of file versions and changes3.

●

Key Git Terminology:

○

Repository (repo): This is equivalent to a project folder where all version-controlled files and their changes are stored3.

○

Commit: This is a snapshot of the files at a specific time. Git compares the current version of files with the previous versions, loads changes, and uploads new versions3. Typically, a commit is accompanied by a note explaining the changes36.

○

Push: This is the action of updating the online repository with the user's committed changes so that everyone has access to those edits3.

○

Pull: This updates a local version of the repository to the current online version, since others may have made changes7.

○

Staging: This is the act of preparing a file for a commit, allowing users to separate changes into separate commits7.

○

Branch: This is when a file has two simultaneous copies, one on the user's local machine and one on the online repository7.

○

Merging: This is the process of incorporating independent edits of the same file into a single unified file6.

○

Conflict: This occurs when multiple people make changes to the same file, and Git is unable to automatically merge the edits6.

○

Clone: This is making a copy of an existing Git repository6.

○

Fork: This is a personal copy of a repository taken from another user6.

●

Best Practices for Using Git: Best practices include making purposeful commits, with each commit addressing a single issue6. Writing informative commit messages is also important6. Users should frequently check that they are up to date by pulling the latest versions and push changes to the common repository8.

●

Setting Up a GitHub Account: The source describes how to sign up for a GitHub account, navigate the website, and fill out profile information. Users can also explore their user settings, notifications, and help files. They are also guided through creating their first repository4.

●

Installing and Configuring Git: The source provides instructions for downloading and installing Git on both Windows and Mac operating systems4. It also describes how to configure Git by setting a username and email4.

●

Linking RStudio with Git and GitHub:

○

The source details how to link RStudio with Git, by confirming the path to the Git executable5.

○

It also describes how to link RStudio to GitHub, by creating an RSA key and adding it to GitHub5.

○

Users can create a repository on GitHub and link it to RStudio by pasting the repository URL into RStudio and creating a new project5.

○

The source also shows how to create a file in the project, stage it, commit it, and push it to the GitHub repository, all from within RStudio5.

●

Linking an Existing Project to Git and GitHub:

○

The source explains how to convert an existing R project to Git version control by using the command line9.

○

It covers how to initialize a Git repository in the project directory and make the initial commit using commands in Git Bash or Terminal9.

○

The source also describes how to link the local repository with GitHub by creating a new repository on GitHub (with the same name) and pushing the local repo using command line instructions9.

○

Finally, the source shows how to clone an existing GitHub repository to a local computer using RStudio9.