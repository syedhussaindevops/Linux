# Users and Groups in Linux

This folder contains Linux user and group management commands used in daily administration tasks.

## Common Commands

whoami                  # Show current logged-in user
id                      # Show user ID and group ID
users                   # Show logged-in users

useradd devopsuser      # Create new user
passwd devopsuser       # Set password for user

usermod -aG sudo devopsuser   # Add user to sudo group
usermod -l newname oldname    # Rename user

userdel username        # Delete user
userdel -r username     # Delete user with home directory

groupadd devops         # Create group
groupdel devops         # Delete group

groups username         # Show groups of user
gpasswd -a user devops  # Add user to group
gpasswd -d user devops  # Remove user from group
