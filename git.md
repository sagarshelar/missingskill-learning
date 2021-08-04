## GIT

**Description**

git is a platform


- to initialise git
```sh
git init .
```
- to clone remote repo into local 
```sh
git clone <remote url>
```
- to add file into stagged
 ```sh
git add <fileName>	
```
- to commit file status
```sh
git commit -m"<messege>"
```
- to check current status of file	
```sh
git status
```

- to change branch
```sh
git checkout <branch>
```
- To push branch on remote
 ```sh
git push <origin> <branch>
```
- to show commit history
```sh
git log
```
- to pull all branches from remote 	
```sh
git pull 
```
- to pull from master/main
```sh
git pull <origin> <master>
```
- To create a new branch
```sh
git branch <name> // created new branch from master
```
- to show cureent working branch
```sh
git branch 
```
- to change branch from one to another	 	
```sh
git switch/ git checkout <branch>
```
- to merge branch(first checkout that branch where we want to merge current branch)
```sh
git merge 
```
- to show changes after commit	
```sh
git show 	
```
- to show changes in file before commit
```sh
git diff
```
- To connect with existing repository
```sh
git remote add origin <remote>
```
- revert all the files to the last commited state
```sh
git checkout -- .
```
- To delete branch
```sh
git branch <name> -d/D // to delete branch
```

**steps to add and commit file from local to repository**

```sh
git status	//shows red 
```
```sh
git add <file>
```
```sh
git status	//shows green
```
```sh
git commit -m"message"
```
```sh
git push origin master
```