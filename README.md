# Fork Custom Commands
Custom Commands Examples for https://git-fork.com/ 

### Open URL by shell
I use a shell file like bellow, because shell command cannot be run directly from Fork Custom Command.
```sh
#!/bin/sh
open $1
```

### Example 1: Open CI Service
##### Menu:
```
Preferences -> Custom Commands -> Add Repository Custom Command
```
##### Config:
```
Script Path: open-by-sh.sh
Parameters: https://travis-ci.com/YourName/$reponame
```

### Example 2: Create Pull Request
##### Menu:
```
Preferences -> Custom Commands -> Add Branch Custom Command
```
##### Config:
```
Script Path: open-by-sh.sh
Parameters: https://github.com/YourName/$reponame/compare/BaseBranchName...$name?expand=1
```

