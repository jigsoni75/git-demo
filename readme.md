- create empty project
- open terminal from intelliJ and hit command `git init`
- after that do `git status` to double check
- if you want change branch name from master to main then use below command
`git branch -M main`
- add .gitignore by command `touch .gitignore`

- `git add .`
- copy contents from https://raw.githubusercontent.com/rdankhara/git-demo/main/.gitignore 
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

- on your main branch you should not find the change which are made in feature-branch
- to get it you
- 1. git fetch (will only download the change from github.com to your local machine)

- 2. `git pull origin main` (that will apply changes downloaded into your branch)


- To delete a branch locally
- `git branch -D feature-HelloWorld`

- to delete a branch on remote
- `git push origin --delete feature-HelloWorld`

