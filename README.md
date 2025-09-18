# Playground
This is a playground for the lab from the Git Branching and Pull Requests lesson from the Software Engineering and DevOps Course at SoftUni.

## Make your changes here

# Git Workflow TODO

## TODO:

- [x] **Fork repo**  
  (no command – do this via GitHub UI by clicking the **Fork** button)  

- [x] **Clone repo**  
```
  git clone <url-of-your-fork>
  cd <repo-folder>
  ```

- [x] **Create a new branch**  
 ```
  git checkout -b my-feature-branch
  ```
- [x] Simulate a conflict scenario
  - [x] Create two branches (dev1 and dev2) from the main branch to act as two dev.
    
    ```
    git checkout main
    git checkout -b dev1
    git checkout main
    git checkout -b dev2
    ```
  
  - [x] Make different changes to the same file on each branch.
  
    ```
    git add README.md
    ```
 - [x] Commit the changes on both branches.
  
    ```
    git commit -m "Dev1: update README.md"
    git commit -m "Dev2: update README.md"
    ```
  - [x] Push the first branch to the remote.
  
    ```
    git push origin dev1
    git push origin dev2
    ```
  - [x] Try to push the second branch to the remote to trigger a conflict.
  
    ```
    git checkout main
    git merge dev1 (first merge)
    git merge dev2 (trigger a conflict)
    ```


- [x] **Make changes to the file**  
  (edit files in your editor: VSCode)  

- [x] **Stage the changes**  
  
 ``` 
  git add <file>
  # or for all files:
  git add .
  ```
  
- [x] **Commit the changes**  
  
  ```
  git commit -m "Add changes for <feature>"
  ```
  
- [x] **Push the changes**  
  
 ```
 git push origin my-feature-branch
 ```
  
- [x] **Create a Pull Request**  
  (no direct git command – do this via GitHub UI: click **Compare & pull request**)  

- [x] **Review and discuss the Pull Request**  
  (happens in GitHub UI through comments and review)  

- [x] **Merge the Pull Request**  
  (happens in GitHub UI: click **Merge pull request**)  

- [x] **Close the Pull Request**  
  (usually closes automatically after merge, or manually via GitHub UI)  

- [x] **Clean up local branches**  
  
``` 
  git checkout main
  git branch -d my-feature-branch
  git push origin --delete my-feature-branch
  ```
  
- [x] **Sync the local repository**  
  (if you haven't added upstream yet → do it once)  
  
 ``` 
 git remote add upstream <url-of-original-repo>
 ```

  then:  
  ```
  git checkout main
  git fetch upstream
  git merge upstream/main
  git push origin main
  ```

- [x] **Update README.md**  
 ```
  git add README.md
  git commit -m "Update README.md"
  git push origin main
  ```
  