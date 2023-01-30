# The Things I Don't Know

## Table of Contents 
- [Git](#git)
  - [Find the current tag](#how-to-find-the-current-tag)
  - [Remove a directory from Git and local](#how-to-remove-a-directory-from-git-and-local) 
  - [How to set username and email in Git](#how-to-set-username-and-email-in-git)
- [Linux Commands](#linux-commands)
  - [Count a word in a file](#how-to-count-occurrences-of-a-word-in-all-the-files-of-a-directory)

## Git
### How to find the current tag?
```sh
  git describe --tags
```

### How to remove a directory from Git and local 
```sh
git rm -r one-of-the-directories // This deletes from filesystem
git commit . -m "Remove duplicated directory"
git push origin <your-git-branch> (typically 'master', but not always)
```
### How to set username and email in git 
```sh
git config user.name "MyName"
git config user.email "MyEmail" 
```

## Linux Commands
### How to count occurrences of a word in a file?
```sh
  grep -ow 'word' filename | wc -l
```
