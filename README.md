# tag-helper
Bash script to ease git tagging process

## Uage
1. Copy the tag-helper file to <WORKING_DIR>/bin/tag-helper.sh
```
e.g. Linux/ Mac
# To create bin directory
mkdir -p ~/bin
# copy file to the bin directory
cp tag-helper.sh ~/bin
cd ~/bin
chmod +x tag-helper.sh

# Updating command to runtime
vim ~/.zshrc
# update the alias - `alias tag=~/bin/tag-helper.sh`
source ~/.zshrc
```
2. Once command helper is configured on the system/machine/laptop then command is set to generate tag version.
3. Use this command from the git repo, either from main or feature branch.
```
     tag -t true # it will generate and push the tag to remote
    # tag -h will give the suggestions about the repo.
```

#### e.g Tag helper is being used and updated on one of my repo. <a href="https://github.com/belwals/docker-learning/tags" target="_blank">Repository</a>
