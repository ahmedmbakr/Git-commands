# Git commands

This files contains the commands needed for Git bash.
You just have to replace the text marked between ```[[...]]``` to fit your  needs.

## Initialize Git user name and password

### How to initalize Git user name globally for all repos

```git config --global user.name "[[your-user-name]]"```

### How to initialize Git email globally for all repos

```git config --global user.email "[[your-email-address]]"```

## Repo cloning

## How to clone repo

```git clone [[project-url]]```

### How to clone repo with submodules

```git clone [[project-url]] --recurse-submodules```

## Repo initialization

### How to initialize a folder in your machine as a new git repository

```git init```

## Frequently used

### How to delete untracked files (new files)

```git clean -xdf```

### How to stage all of the files

```git add .```

### How to stage a specific file

```git add [[file-path-relative-to-repo-root]]```

### How to stage files that using regex

```git add [[regex]]```

Example: To stage all the c files in the working directory,  ```git add *.c```

### How to show the status of the files in the repo

The status shows the modified, the added, the deleted files. For each of the files it shows if the files are staged or not

```git status```

### How to reset changes for a file

```git checkout --[[file-name]]```

### How to reset all changed files in the working directory

```git reset --hard```

## Repo's remote

### How to modify remote for a repo

```git remote set-url [[origin-name]] [[new-remote-url]]```

Example:
```git remote set-url origin [[new-remote-url]]```

### How to add a new remote for a repo

```git remote add [[origin-name]] [[new-remote-url]]```

Example:
```git remote add origin [[new-remote-url]]```

## Advanced Topics

### How to enable CRLF by default

```git config --global core.autolf false```
```git config --global core.autocrlf true``

### How to force git to rescan all the project

```rm .git/index```

## Useful links

### [Gitlab bash documentation](https://docs.gitlab.com/ee/gitlab-basics/start-using-git.html
)