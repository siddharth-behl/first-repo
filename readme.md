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

git log --grep="<text>"- it will search the version which is having <text> in the commit message. 
git log -S <type_text_you_want_to_search_in_any_file>- it will give you info only about the files from which the text you entered is added or removed
git log --since=<date>- all the data after the <date>
git log --until=<date>- all the data before the <date>
git log --author=<name>- to get data of a particular author
git log --no-merges- By using git log --no-merges, you filter out these merge commits, giving you a clearer view of the commit history with only the non-merge commits displayed. This can be particularly useful when you're trying to understand the chronological order of changes, track down when specific features or bug fixes were implemented, or simply reviewing the history of a project without the distraction of merge commits.
git remote -v - to check if the remote repo  is linked to local repo or not -v is to check which repo is linked to it and it also gives the link to repo
git branch - to check all the branches
git branch <name_of_branch> -  to create a new branch
git checkout <branch_name>- to get to that branch you have created to specifically work on it.
when a file is not tracked it is untracked then when we do git add then it goes to the staging area then when we commit the file then it gets tracked 