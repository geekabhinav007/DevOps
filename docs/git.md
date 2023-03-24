# GIT Tutorial for MST 1 (According to Syllabus)

## GIT Basics

### What is GIT?

GIT is a version control system. It is a tool to manage your source code history. It allows you to keep track of your work and helps you to easily collaborate with others.

### Why do we use GIT?

- It allows you to keep track of your work.

- It allows you to easily collaborate with others.

- It allows you to easily revert to a previous version of your code.

- It allows you to easily share your code with others.

### What is a repository?

A repository is a directory that contains your project's files and each file's revision history. You can communicate with a remote repository using the git fetch, git push, and git pull commands.

## Some Basic GIT Commands

### git init

The git init command creates a new Git repository. It can be used to convert an existing, unversioned project to a Git repository or initialize a new, empty repository.

### git --bare init

The `git --bare` command is used to create a bare Git repository. A bare repository is a Git repository that does not have a working directory, and it only contains the Git repository files, such as the .git directory and the objects that make up the repository's history. A bare repository is typically used as a central repository for sharing code between developers or as a remote repository for deployment.

To create a bare Git repository using the `git --bare` command, navigate to the directory where you want to create the repository and run the following command:

```bash
git init --bare
```

This will create a new bare Git repository in the current directory. The `--bare` option specifies that the repository should be bare.

Once you have created the bare repository, you can push code to it using the git push command. For example, if you want to push the master branch to the origin remote repository, you would run the following command:

```bash
git push origin master
```

This would push the master branch to the origin remote repository, which could be a bare repository or a repository with a working directory.

>> In summary, the `git --bare` command is used to create a bare Git repository, which is a repository that does not have a working directory and is typically used as a central repository for sharing code between developers or as a remote repository for deployment.

The `git status -s` command is used to display a short summary of the current state of the Git repository, including the status of any modified, added, or deleted files in the working directory.

Here's a breakdown of what each part of the command does:

- `git status`: This is the command used to display the current status of the Git repository.
- `-s`: This option specifies that a short summary should be displayed.

When you run the git status -s command, Git will display a two-column output that shows the status of each file in the repository. The first column shows the status of the file in the staging area, and the second column shows the status of the file in the working directory. The status codes are as follows:

- `M`: The file has been modified in the working directory.
- `A`: The file has been added to the staging area.
- `D`: The file has been deleted from the working directory.
- `R`: The file has been renamed.
- `C`: The file has been copied.
- `U`: The file is unmerged due to a conflict.

The `git log` command is used to display the commit history of a Git repository.

By default, the `git log` command shows the following information for each commit:

- SHA: The unique identifier for the commit.
- Author: The name and email address of the person who made the commit.
- Date: The date and time that the commit was made.
- Commit message: The message that was provided when the commit was made.
The output is displayed in reverse chronological order, with the most recent commit shown first.

```bash
kumar@g3:~/kumar-repo$ git log
commit 0195fed22d1747573609201fa77a3418c0ef7623 (HEAD -> master)
Author: Kumar Abhinav <kumar@example.com>
Date:   Sat Mar 25 02:55:41 2023 +0530

    Intial Commit by user Kumar
kumar@g3:~/kumar-repo$ 
```
