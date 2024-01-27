## Git Tag Helper

This Bash script simplifies the git tagging process by providing an easy-to-use command for generating and pushing tags to the remote repository.

### Usage

1. Copy the script to the bin directory:
   * Linux/Mac:
```
# Create bin directory if it doesn't exist
mkdir -p ~/bin
# Copy the script to the bin directory
cp tag-helper.sh ~/bin
cd ~/bin
chmod +x tag-helper.sh
```
2. Update the command for runtime:
   * Open your shell configuration file (e.g., ~/.zshrc) using a text editor.
     ```
     vim ~/.zshrc
     ```
   * Add the following alias to the file:
     ```
     alias tag=~/bin/tag-helper.sh
     ```
   * Save the file and source the updated configuration:
     ```
     source ~/.zshrc
     ```
3. Generate and push tags:
   * Once the command helper is configured, you can use the following command from the git repository (main or feature branch):
     ```
     tag -t true # generates and pushes the tag to the remote repository
     ```
   * Use tag -h to get suggestions about the repository.
4. Example:
   * Tag helper is being used and updated on one of my repositories.

Feel free to customize the script or the alias according to your preferences. This script enhances the efficiency of managing tags in your Git workflow.
