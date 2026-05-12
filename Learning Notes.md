# **Git Commands**



**git init** - Initilizing git in the Current Directory.



**git clone https://github.com/repository.git** - for cloning the project(the project link is paased in the command) locally.



**git remote add origin https://github.com/yourusername/project-name.git** - This Command is used to Connect a local repo to Remmote Repository.

**git push -u origin main** - After connecting remote repository, we are pushing code to that remote repo. -u stands for Upstream, that remember the Orgin(Repo Connection Everytime).



**git status** - checking the git status, it will show, what files are modified, created, deleted, what needs to be added to "Staging".



**git add --all** - It will ADD all the file to "Staging".

**git add .** - it will add the all files in current Directory.

**git add Thisfile** - It will add the mentioned file name (Thisfile) to "Staging".

**git add \*** - Adds all tracked and untracked files in the current directory. But Doesn't include deleted files.

**git add \*txt** - It will add the all the mentioned file type(txt, jpg, doc, java, anyfiletype) to "Staging".



**git reset** - it will reset the files that are in "Staging" into working Directory.



* &#x20;   **git reset --soft HEAD\~1** - Removes the last commit, Keeps all changes in the staging area.
* &#x20;   **git reset --mixed HEAD\~1** - Removes the last commit, Unstages the changes.
* &#x20;   **git reset --hard HEAD\~1** - Deletes the last commit, Removes all staged changes, Deletes all working directory changes. Resets your project exactly to the previous commit. You made a               				 bad commit and want to completely erase it.
* &#x20;   **git reset --hard** - Deletes all uncommitted changes, Keeps all commits intact. if you messed up your working files and want to go back to the last committed state.



**git commit -m "This Commit Message"**  - This is used for "Commit" the all files in the "Staging". the Commit Message is Mentioned between the Quotation " ".



**git rm ThisFile** - This will remove or delete the mentione file (ThisFile can be any filename) name also "Stage" the changes, in single command. we don't need to "Stage" the Deleted status Individually.



* &#x20;  **git rm -f filename.txt** - removes the file forcefully.



* &#x20;  **git rm -cached filename.txt**  - removes the file in staging area, but keeps in working Directory.



* &#x20;  **git rm -r <Folder**>  - This command delete the folder and its Contents. <Folder> - this can  be any folder you want to delete. -r stands for recursively.



**git log** - This shows the logs of "Commits". and also Commit ID's



* &#x20;  **git log --oneline** - This will show the oneline version "Commit" logs and their Shorted ID's.



**git branch** - list out all the branches present in the repository.



* &#x20;  **git branch <newBranchName>** - Creates the New Branch we Mentioned. This new inherit the contents of the Current Branch(The branch that we have in when we are created the new Branch)



* &#x20;  **git checkout <newBranchName>** - Switch to the Branch we Mentioned.



**git merge main -m** "Merging main branch into Current branch"

**git checkout <Commit ID>** - This command is used for Changing the this to (Commit ID) version of project.

**git diff <Commit ID> <Commit ID**> - This command is used for Seeing the difference and Changes between to Commits.



**Press 'Q' for exit Git Log.**



**git push orgin main** - This pushes the commits to Remote Repository "main" Branch. also it creates the  branch in remote repository and push the code. in if it not present in remote repo.



**git fetch**   - It fetch the latest change in the  current Branch in remote repository into local Directory. use "git merge " to reflect those changes is in local directory.



**git pull** - this Command is used for fetch and merge the the latest changes in the remote repository into local Directory. in Current Branch.



**git restore <filename or Directory>** - This command is used for restoring the file or directory or whole repo to it's previous commits, but changes we made should be staged or committed.



**git restore .**  - restore all files (whole repo) to it's previous commit.



**git restore --staged <filename or Directory or whole repo>** - This command is used for restore all the staged( specific file or Directory or whole repo) to its previous Commits.



**git stash** - the unstaged changes can be stored in temporary file. then it can be retrieved.

**git stash pop** - removed stash and restore the changes.



**git stash pop stash@{0}** - remove the specific stash file (stash@{0}), from the temporary file then restore the changes.



**git stash apply** - apply the changes, but keep stashed changes in the temporary file.



**git stash apply stash@{1}** - apply the changes in the specified stash file (stash@{1}), also keep that file in temporary file.



**git stash drop** - removes/drop all the changes in the temporary file.



**git stash drop stash@{1}** - removes/drop specified stash file (stash@{1}) the changes in the temporary file.



**git revert <Commit ID>** - is used to undo a commit safely by creating a new commit that reverses the changes.It does not delete history from Commit History.

**git rebase <branchName>** - To update your branch with the latest changes from another branch (often main or develop) without creating a merge commit.Keeps history linear and clean, unlike git merge which introduces extra merge commits.

