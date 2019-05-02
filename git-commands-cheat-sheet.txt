1. git checkout -n new_branch_name
Create a new branch from current branch, and stays in the new branch, continue your work from here

2. git branch
In the console, a list of branches will show up

3. git branch -d branch_name
Delete branch that is no longer needed, this branch needs to be fully merged

4. git branch -D branch_name
If the branch is not fully merged and you still want to delete the branch

5. git rebase remote_repo_name branch_name_you_want_to_rebase_against
Rebase your current work on another branch, it will give you clear commit history

6. git rebase -i HEAD~some_number
Used when you want to reorder your commits history

7. git fetch remote_name
Fetch all of it from remote repo, usually used with git rebase command. A good habit is to keep rebase with
master to have a clear commit history, and avoid possible merge conflicts which may become so complex to 
solve.

8. git clone HTTPS_address Or SSH_address
Clone the remote repo to your local computer

9. git push --set-upstream remote_name branch_name_you_want_to_have_in_remote_repo
 Set up tracking branch in remote repo for your local branch, you can use this command with git checkout command

10. git diff
Show all the differences in current branch that haven't been added yet
    git diff file_name
    Only show differences in this file 
