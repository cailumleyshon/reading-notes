# Week 1 Class 3 - Revisions and the Cloud ☁️
- - - - - - - - - - - - - - - - - - - - - - - 
- - - - - - - - - - - - - - - - - - - - - - -

## "What is Version Control?"
- - - - - - - - - - - - - - - -
Version Control is a system that allows you to revisit various versions of a file or set of files by recording changes. From this, we have a LVS (Local Version Control) which entails one database on your hard disk/own computer that stores changes to files. Multiple developers working on multiple local version controls caused the collaberation process to be streamlined into a much more efficient version control,
CVS (Centralised Version Control) which entails a single server storing all changes and file versions, which can be accessed by various clients. However, being on a single server, this is susceptible to going down. The DVC (Distributed Version Control) addresses the risk of issue with a CVS (server down) and LVS (corruption) and allows for multiple mirrored repositories and enables the use of multiple workflows between programmers. An example of a DVCS is **Git**.
- - - - - - - - - - - - - - - - -

## "What is 'cloning' in Git?"
- - - - - - - - - - - - - - - - -
Cloning in Git is the process of making a copy of an existing Git repository from a remote server. This copy includes all versions of all files in the project. When you clone a repository, Git not only creates a local copy but also initializes a hidden .git directory inside it, which contains all the version history and data for the project.

By using the git clone command followed by the repository's URL, you can create this copy. For example:
```
~ git clone git@github.com:cailumleyshon/youre-a-git.git
```
This command will create a directory named "youre-a-git" and download all the project's files and history into it. It will also automatically check out the latest version of the project, so you can start working with it immediately.

If you want to specify a different name for the directory in which the repository will be cloned, you can use the following format:
```
~ git clone git@github.com:cailumleyshon/youre-a-git.git Projects
```
In this case, the copy of the repository will be placed in a directory named "Projects".

In summary, cloning in Git is the process of creating a local copy of a remote Git repository, including all its files and version history, using the git clone command. This allows you to work on the project locally, make changes, and collaborate with others without affecting the original repository on the remote server.
- - - - - - - - - - - - - - - - - -

## "What is the command to track and stage files?"
- - - - - - - - - - - - - - - - - - 
To track and stage files in Git, you use the `git add` command. Here's how you do it:

To track and stage a single file, you can use the following command format:

```
~ git add filename
```

For example, if you want to track and stage a file named "example.txt," you would use:
```
~ git add example.txt
```

To track and stage all files in a repository, you can use the wildcard `*` like this:
```
~ git add *
```

After using these commands, the files you've specified will be tracked and staged for committing. When you check the status of your Git repository using `git status`, it will show you information about the changes that are ready to be committed. For instance:
```
On branch master

Changes to be committed:

  (use "git reset HEAD ..." to unstage)
new file: example.txt
```

This information indicates that there are changes to be committed, and the specified file(s) have been staged and are ready to be included in the next commit.
- - - - - - - - - - - - - - - - - - -

## "What is the command to take a snapshot of your changed files?"
- - - - - - - - - - - - - - - - - - - -
To take a snapshot (create a commit) of your changed files in a Git repository, you use the `git commit` command. Here's how you do it in the terminal:

```
~ git commit -m "Your commit message here"
```

Replace `"Your commit message here"` with a concise and meaningful message that describes the purpose of the commit.

For example, if you're adding a new feature to your code, you might use a commit message like:

```
~ git commit -m "Add new feature X"
```
Another commit argument that can be used is:

```
~ git commit -a
```
which adds **all** modified files, without a message.

After running this command, Git will create a new commit with the staged changes, and it will be saved in the version history of your repository. The commit message you provided helps you and others understand what this particular commit represents.

Commits are like snapshots of your code at a specific point in time, and they allow you to track the history of changes in your Git repository.
- - - - - - - - - - - - - - - - - - - 

## "What is the command to send your changed files to Github?"
- - - - - - - - - - - - - - - - - - - 
Finally, you would **push** changes to a remote repository. We will discuss remote repositories in more depth in the next section. For now, we will look at a general overview of pushing changes to remotes.

Example:

```
~ git push origin master
```
This command pushes changes from the local “main” branch to the remote repository named “origin” and will be updated in GitHub.

For cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “main” to your local repository. However, these names can be changed by the user.
- - - - - - - - - - - - - - - - - - - - -
