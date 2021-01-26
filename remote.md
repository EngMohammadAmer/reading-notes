[Home](README)

# Remotes

## Seeing Your Remotes

By running the git remote command, you can view the short names, such as “origin,” of all specified remote handles.

By using git remote -v, you can view all the remote URLs next to their corresponding short names.

## Adding Remotes

To create a new remote Git repository with a short name, use the following format:

git remote add shortname url

## Fetching

Fetching entails pulling data that you don’t have from a remote project.

git fetch [remote-name]

## Pushing

To push your changes “upstream” for sharing, you would use the following git push command format:

git push [remote-name][branch-name]

## Renaming/Removing Remotes

### Rename

To rename a remote’s short name, use the git remote rename command.

### Remove

To remove a remote for whatever reason (e.g., a contributor has left the team, the server has moved), simply use the git remote rm command


