# Git and GitHub and co. <br> <br>
---
---
### **1. Install Git(Bash)** <br>
### **2. Learn main commands to manipulate.** <br>
### **3. Create Git repository and memorize main commands.** <br>
### **4. Sign up in GitHub and create remote GitHub repository.** <br>
### **5. Find out how to connect local Git repositories and remote GitHub ones.** <br>
### **6. Git status, git log, git add, git commit -m, hashes, HEAD, statuses: untracked, modified, staged etc.** <br>
### **7. How to write proper commit's messages.** <br>
### **8. README.md files, learn creating this type of files and use it smartly. MARKDOWN.** <br>
### **9. Use Mermaid language schemes.** <br> <br>
### **10. Use `git commit --amend --no-edit` or `git commit --amend -m "new message"` to edit the last commit(HEAD).** <br>
### **11.`git restore --staged <file>` and `git reset --hard <commit hash>` and `git restore <file>`** <br>
### **12. `git diff` and `git diff --staged` to see the difference.** <br>
### **13. `git diff` shows you the differences between modified; `git diff --staged` shows the differences btw in staged changes.
### and  there's `git diff <hash> <another hash>` that shows the changes btw commits with these hashes** <br>
### **14. Create .gitignore file to ignore some files or directories. It will not be tracked. And commit .gitignore before that ** <br>
### Use special rules to do that. Like *, **, /, #, ?, file[0-9].txt for example. <br>
### **15. To copy a remote repository use `git clone + <SSH-key of the repository>`. It connect a remote rep. and a local rep. automaticaly.** <br>
### **16. `git branch` shows you all branches. `git branch <branch_name>` to create a branch. `git checkout <branch_name>` to switch to a new branch.**
### **`git checkout -b <branch-name>` to create and switch to a new branch. ** <br>
### **17.`git diff <branch_name> <anpther_branch_name>` shows the difference btw these branches. Or use a hash instead of branch_name.** <br>
### **18. Use ~ to refer to the previous commits. For example: `git diff main~3 main` to compare the last commit(HEAD) in main branch and 4th commit from the end.** <br>
### **19. `git merge <branch_name>` to merge(join) two branches together. For deleting a branch use a command `git branch -D <branch_name>` or a lighter variant with flag `-d`.** <br>
### **20. For adding a branch to GitHub use `git push -u origin <not-a-main-branch>`. 
### **21. To merge your branch with the main in GitHub use PULL REQUEST by the link while push it first time or use GitHub interface to pull request, review code, comment it and cancel or merge it with the main branch.**<br>
### **22. `git pull` to get the changes from the remote repository.
### **23. If two branches are without conflicts and all commits may be put in one chain, these branches can be merged in fast-forward mode. You can turn the mode off using the flag `--no-ff`. **
### **`git merge --no-edit --no-ff <branch-name>`
### **24. `git push --force` can push your local branch to the remote one.WARNING: can be deleted some commits or the branch can be broken. Use it wisely.**
### **25. There are several types of work with branches:**
### **feature branch workflow - when every new feature or change is supposed to be in a new branch and can be merged in the main till completion. **
### **git flow - more complicated variant, created more branches and all commits are divided on different types: fix,feature etc. Different commits are located in different branches.**
### **trunk-based - populat in big companies, it is similar to feature branch workflow. Participants often merge their code in the main. E.g every day.**
### 
---
---


```mermaid
graph LR;
  untracked -- "git add" --> staged;
  staged    -- "???"    --> tracked/comitted;

%% the arrow without any text for example:
  A --> B;
```