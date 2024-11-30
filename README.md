# Auto-Generated Git Tag Script
This script automates the process of generating Git tags based on the last commit timestamp and branch name, simplifying version control in your Git workflow. This script is ideal for developers familiar with Git.

## Benefits:
- Reduce errors in manual tag creation.
- Ensure consistent tag format across branches.
- Improve traceability between versions.

## Installation

1. Copy the script to the bin directory:
   *  Linux/Mac:
      ```
      # Create a user-specific bin directory if it doesn't exist
      mkdir -p ~/.local/bin
      # Copy the script to the bin directory
      cp version_script.sh ~/.local/bin
      cd ~/.local/bin
      chmod +x version_script.sh
      ```
2. Update the command for runtime:
   * Open your shell configuration file (e.g., ~/.zshrc) using a text editor or by below command.
   * Add the following alias to the file:
     ```
     alias tag=~/bin/version_script.sh
     ```
   * Save the file and source the updated configuration:
     ```
     source ~/.zshrc
     ```

## Usage

1. Generate and push tags:
   * Once the command helper is configured, you can use the following command from the git repository (main or feature branch):
     ```
     tag -t true # This generates and pushes the tag to the remote repository.
     ```
   * Use tag -h to get suggestions about the repository.
2. Default behavior: Without the -t option, the script only generates the tag locally and does not push it.
3. Branch name handling:
   * Main/Master: Tags will be in the format YYYYMMDDHHMMSS.<commit_hash>
   * Feature Branch: Tags will be in the format YYYYMMDDHHMMSS.<commit_hash>-<branch_name>

## Customization:
The script can be customized to modify the tag format or behavior (advanced users).

## Example:
This script is used in my repository <a href="https://github.com/belwals/docker-learning/tags" target="_blank">Docker Learning</a>, to automatically generate tags with each commit and push them to the remote repository, ensuring clear version tracking and traceability.

Feel free to adapt the script and alias to your specific workflow preferences.
