 ### Helpful Stuff
  
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

