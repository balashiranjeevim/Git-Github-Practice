# **Git Commands**



**git init** - Initilizing git in the Current Directory.



**git clone https://github.com/repository.git** - for cloning the project(the project link is paased in the command) locally.



**git status** - checking the git status, it will show, what files are modified, created, deleted, what needs to be added to "Staging".



**git add --all** - It will ADD all the file to "Staging".

**git add .** - it will add the all files in current Directory.

**git add Thisfile** - It will add the mentioned file name (Thisfile) to "Staging".

**git add \*** - Adds all tracked and untracked files in the current directory. But Doesn't include deleted files.

**git add \*txt** - It will add the all the mentioned file type(txt, jpg, doc, java, anyfiletype) to "Staging".



**git reset** - it will reset the files that are in "Staging" into working Directory.



* &#x20;   **git reset --soft HEAD\~1** - Removes the last commit, Keeps all changes in the staging area.
* &#x20;   **git reset --mixed HEAD\~1** - Removes the last commit, Unstages the changes.
* &#x20;   **git reset --hard HEAD\~1** - Deletes the last commit, Removes all staged changes, Deletes all working directory changes. Resets your project exactly to the previous commit.You made a               				 bad commit and want to completely erase it.
* &#x20;   **git reset --hard** - Deletes all uncommitted changes, Keeps all commits intact. if you messed up your working files and want to go back to the last committed state.



**git commit -m "This Commit Message"**  - This is used for "Commit" the all files in the "Staging". the Commit Message is Mentioned between the Quotation " ".

**git rm ThisFile** - This will remove or delete the mentione file (ThisFile can be any filename) name also "Stage" the changes, in single command. we don't need to "Stage" the Deleted status Induvidually.



**git rm -f filename.txt** - removes the file forcefully.



**git rm -cached filename.txt**  - removes the file in staging area, but keeps in working Directory.





