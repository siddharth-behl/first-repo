git status - tells u about the status of the file
git init - to initialize a git 
git config --lists  - to list the user details and some extra settings
git commit -m <message> -  to commit a file to github
git log - to see the commited file messages and details like the author and the date.
git diff-  to see the difference in the file before staging(means you just edited the file) and after staged file(means the file which was staged earlier ) 
git diff --cached -  to see the difference in the file from previous version after the file is staged 
git checkout <uid> --<file_name (use * for all files)> - to get the previous version files
git checkout master -  to get back to the latest version of the file you have created
git restore <filename or . for all> - to restore the particular file or all files to the latest working version 
git show <unique-commit-id>- to
git restore --staged <filename>- to remove from staging phase .
git restore --worktree <filename> -  to remove the changes from the file before staging process
when a file is not tracked it is untracked then when we do git add then it goes to the staging area then when we commit the file then it gets tracked 