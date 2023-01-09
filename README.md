# the-things-i-dont-know

## Table of Contents 
- [Git](#git)
- [Linux Commands](#linux-commands)

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
### How to count occurrences of a word in all the files of a directory?
```sh
  grep -ow 'word' filename | wc -l
```
