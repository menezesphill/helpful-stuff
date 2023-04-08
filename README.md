 # Helpful Stuff
  
 ### GIT
 
  Find deleted files in the project historical data
  
  ```csh
  git log --all --full-history -- "**/file-name.*"
  ```

  Create a new branch from uncommited changes
  
  ```csh
  git switch -c <new-branch>
  ```

  Change remote URL
  
   ```csh
  git remote set-url origin https://git-repo/new-repository.git
   ```
  
  Undo staged commit
  
  ```csh
  git reset HEAD~1
   ```
  
  Create new git upstream
  
 ```csh
 git push --set-upstream origin master
  ```
  
 Merge repos
 
  ```csh
 git merge target_branch --allow-unrelated-histories
  ```
  
 Resolve different history

```csh
-- Remove the history from 
rm -rf .git

-- recreate the repos from the current content only
git init
git add .
git commit -m "Initial commit"

-- push to the github remote repos ensuring you overwrite history
git remote add origin git@github.com:<YOUR ACCOUNT>/<YOUR REPOS>.git
git push -u --force origin master
```

### DOCKER

Access container shell

```csh
docker run -it image_name sh
```

Stop all instances

```csh
docker kill $(docker ps -q)
```

Delete all instances

```csh
docker rm $(docker ps -a -q)
```
Chance Branch name 

``` csh
git branch -m master main
git fetch origin
git branch -u origin/main main
git remote set-head origin -a
```
