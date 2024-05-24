git branch -  to check all the branches existing in the git
git status - tells u about the status of the file
git init - to initialize a git 
git config --lists  - to list the user details and some extra settings
git commit -m <message> -  to commit a file to github
git log - to see the commited file messages and details like the author and the date.
git diff-  to see the difference in the file before staging(means you just edited the file) and after staged file(means the file which was staged earlier ) 
git diff --cached -  to see the difference in the file from previous version after the file is staged 
git checkout -b <branch_name> <uid> --<file_name (use * for all files)> - to get the previous version files use -b to make a new brach name and you can then use your branch name to access that version of file easily.
git checkout master -  to get back to the latest version of the file you have created
git restore <filename or . for all> - to restore the particular file or all files to the latest working version 
git show <unique-commit-id>- to
git restore --staged <filename>- to remove from staging phase .
git restore --worktree <filename> -  to remove the changes from the file before staging process
git reset <--hard><OR><--soft> HEAD^ - this will remove the latest version of the commit and will send you back to the previous version now if you use soft it will just uncommit the version but will keep the data intact but if you use hard it will remove the data too from the file that was changed in the particular version .
Using `--soft` will uncommit the changes but keep them intact, while `--hard` will remove the changes from the working directory as well.
git log -p -<number of versions you want to see> - this will help you to check a particular amount of versions from latest to old 
git log --stat - this is used to get basic summary of the versions.
git log --pretty=oneline - to check all the version messages branches and uid in one line .
git log --pretty=format:"%h - it was generated %ar by %an  and version is ---->%s" - here %h means hash or the <commit-uid> .
%ar-relative time - it is the time of the version was added relative to the time now
%an - author name-  to see what is the user.name
%s- it is the string or the message you gave while commiting.

when a file is not tracked it is untracked then when we do git add then it goes to the staging area then when we commit the file then it gets tracked 