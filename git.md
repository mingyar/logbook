# How to delete a remote branch?
````
git push origin --delete your_branch
````
# How do I do an initial push to a remote repository with Git?
````
mkdir my_project
cd my_project
touch .gitignore
git init
git add .
git commit -m "Initial commit"
git remote add origin youruser@yourserver.com:/path/to/my_project.git
git push origin master
````
# How can I determine the URL that a local Git repository was originally cloned from? 
If you want only the remote URL, or if your are not connected to a network that can reach the remote repo:
````
git config --get remote.origin.url
````
If you require full output and you are on a network that can reach the remote repo where the origin resides:
````
git remote show origin
````
https://stackoverflow.com/questions/4089430/how-can-i-determine-the-url-that-a-local-git-repository-was-originally-cloned-fr
# How to change the URI (URL) for a remote Git repository?
````
git remote set-url origin new.git.url/here
````
# How to undo the last commit?
````
git reset --soft HEAD~1
````
