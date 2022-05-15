- create empty project
- open terminal from intelliJ, verify the path does not have (master) or (main) if it is then you have created a folder inside another git project, check for the .git folder in any of the parent folder and either create new folder outside of parent or remove un necessary .git folder from tha parent directory may be inside your c:\Users\(YourUserName) 
- initialize git project using command `git init` ,
- after that do `git status` to double check
- if you do git init and you see (master) instead of main, then rename your branch to main using command
    `git branch -M main` check point configure default branch name to permanently apply change
- add .gitignore by command `touch .gitignore`

- copy contents from https://raw.githubusercontent.com/rdankhara/git-demo/main/.gitignore
- `git add .`
- `git commit -m 'initial commit'`

- create git repository on git hub

- copy command of git remote add origin (double check url https or ssh) , go for ssh only if you have setup ssh configuration

- `git push origin main`

- create new branch using command `git checkout -b name-of-branch`
- apply your changes
- add using `git add .`
- commit using `git commit -m 'message'`
- push using `git push origin name-of-branch`
- create pull request by clicking the link
- merge it when it gets approval on git hub

- on your local verify that main is not modified by command `git checkout main`
  (This will not work if you have modified anything on your local branch, so you can check it using git status, if you find any changes then either commit or revert using git restore and then retry `git checkout main`)
- on your main branch you should not find the change which are made in feature-branch
- to get it you
- 1. `git fetch` (will only download the change from github.com to your local machine)

- 2. `git pull origin main` (that will apply changes downloaded into your branch)

- To delete a branch locally
- `git branch -D feature-HelloWorld`

- to delete a branch on remote
- `git push origin --delete feature-HelloWorld`

- configure default branch name (this is one time change)
- `git config global --init.defaultbranch main`

- information about configure ssh key https://docs.github.com/en/authentication/connecting-to-github-with-ssh/about-ssh 
