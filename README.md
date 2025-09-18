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

- [ ] **Create a new branch**  
 ```
  git checkout -b my-feature-branch
  ```
  
- [ ] **Make changes to the file**  
  (edit files in your editor: VSCode)  

- [ ] **Stage the changes**  
  
 ``` 
  git add <file>
  # or for all files:
  git add .
  ```
  
- [ ] **Commit the changes**  
  
  ```
  git commit -m "Add changes for <feature>"
  ```
  
- [ ] **Push the changes**  
  
 ```
 git push origin my-feature-branch
 ```
  
- [ ] **Create a Pull Request**  
  (no direct git command – do this via GitHub UI: click **Compare & pull request**)  

- [ ] **Review and discuss the Pull Request**  
  (happens in GitHub UI through comments and review)  

- [ ] **Merge the Pull Request**  
  (happens in GitHub UI: click **Merge pull request**)  

- [ ] **Close the Pull Request**  
  (usually closes automatically after merge, or manually via GitHub UI)  

- [ ] **Clean up local branches**  
  
``` 
  git checkout main
  git branch -d my-feature-branch
  git push origin --delete my-feature-branch
  ```
  
- [ ] **Sync the local repository**  
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
  