# the-things-i-dont-know

## Table of Contents 
- [Git](#git)

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
