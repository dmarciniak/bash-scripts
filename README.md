# bash-scripts
Useful bash scripts

Testing on Ubuntu 18.04

## Installation
```
git clone https://github.com/dmarciniak/bash-scripts/
cd bash-scripts/bin
chmod u+x *
echo "export PATH=\$PATH:$(pwd)" >> ~/.bashrc
bash
```
## pin
Script create alias for cd command to current location

Use ```pin <alias_name>```

Example:
```
dmarciniak@laptop:~$ cd Projects/
dmarciniak@laptop:~/Projects$ pin proj
dmarciniak@laptop:~/Projects$ cd
dmarciniak@laptop:~$ proj
dmarciniak@laptop:~/Projects$ 
```

## unpin
Script remove alias for cd command for current location or for alias name given in first parameter

Use ```unpin``` or ```unpin <alias_name>```

Example:
```
dmarciniak@laptop:~/Projects$ proj
dmarciniak@laptop:~/Projects$ cd
dmarciniak@laptop:~$ proj
dmarciniak@laptop:~/Projects$ unpin
dmarciniak@laptop:~/Projects$ cd
dmarciniak@laptop:~$ proj

Command 'proj' not found

```
