# The Things I Don't Know

## Table of Contents 
- [Git](#git)
  - [Find the current tag](#how-to-find-the-current-tag)
  - [Remove a directory from Git and local](#how-to-remove-a-directory-from-git-and-local) 
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
## Linux Commands
### How to count occurrences of a word in a file?
```sh
  grep -ow 'word' filename | wc -l
```
