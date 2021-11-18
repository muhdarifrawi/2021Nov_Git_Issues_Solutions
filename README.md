## Issues and Solutions for Git

## Initiated in wrong folder 
### Description and background
Git was initialised in unintended folder. Want to move git to parent foldder which is the intended location.

### Solution
Source: [My Git repository is in the wrong root directory. Can I move it? (../ instead of ./)](https://stackoverflow.com/questions/1918111/my-git-repository-is-in-the-wrong-root-directory-can-i-move-it-instead-of)

Run the following code:
```BASH
$ mv .git ../
$ cd ..
$ git add .
$ git commit -m "your comments" 
```

### Errors Encountered
#### fatal: ...... failed: Permission denied
`fatal: ...... failed: Permission denied`

Most likely there were terminals that were still using the directory. Close them and only run the commands in one terminal.

Source: [Changing case of Folder via Git bash on Windows](https://stackoverflow.com/questions/14578680/changing-case-of-folder-via-git-bash-on-windows)