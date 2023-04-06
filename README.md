# The Things I Don't Know

## Table of Contents 
- [Git](#git)
  - [Find the current tag](#how-to-find-the-current-tag)
  - [Remove a directory from Git and local](#how-to-remove-a-directory-from-git-and-local) 
  - [How to set username and email in Git](#how-to-set-username-and-email-in-git)
  - [Compare two git branches](#compare-two-git-branches)
- [Linux Commands](#linux-commands)
  - [Count a word in a file](#how-to-count-occurrences-of-a-word-in-all-the-files-of-a-directory)
- [Docker](#docker)
	- [Procceed and delete all stopped containers](#procceed-and-delete-all-stopped-containers)
- [Redis](#redis)
	- [Get information about redis server](#get-information-about-redis-server)

## Git
### fatal: transport 'file' not allowed
Issue link: https://vielmetti.typepad.com/logbook/2022/10/git-security-fixes-lead-to-fatal-transport-file-not-allowed-error-in-ci-systems-cve-2022-39253.html
Solution
```sh
git config --global protocol.file.allow always 
```

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
### Compare two git branches
```sh
# Using double dots
# Show all the commits that branch2 has that are not in branch1

git diff branch1..branch2

# Using triple dots
# Compare the Head of branch 2 with the common ancestor of two branches 
git diff banch1...branch2

```


## Linux Commands
### How to count occurrences of a word in a file?
```sh
  grep -ow 'word' filename | wc -l
```

## Docker
### Procceed and delete all stopped containers
```sh
docker container prune -f 
```

## Redis 
### Get information about redis server
```sh 
INFO server 
```
