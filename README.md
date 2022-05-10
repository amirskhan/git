# Git tutorial

## Configure Git
Configure local Git client with username and email address. Omit --global to keep username and email only to the specific git repository.
git config --global user.name "your_github_username"
git config --global user.email "your_github_email"

## Adding a local repository to GitHub
Initialize the local directory as a Git repository.
git init -b main

Add the files in your new local repository.
git add .

Stage and commit all the files in your project
git add . && git commit -m "initial commit"

Sets the new remote
git remote add origin  <REMOTE_URL>

Verifies the new remote URL
git remote -v

Push the changes in your local repository to GitHub.com. 
git push origin main

Username: <type your username>
Password: <type your password or personal access token (GitHub)>

Cache the given record in your computer to remembers the token
git config --global credential.helper cache
  
To delete the cache record
git config --global --unset credential.helper
git config --system --unset credential.helper
