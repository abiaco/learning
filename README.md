# learning
test environment for learning git commands!

A few basic commands:

  -> git status: shows you the status of the curent git repository, the changes you made, new files added, untracked files etc. as well as the difference between local and remote.
  -> git clone <repository>: clones repository into your local directory!
  -> git add <filename>: adds a local file to the git repository.
  -> git rm <filename>: removes file from repository.
  -> git commit -m <message>: commits changes, setting the commit message to <message>
  -> git commit --amend: change the commit message of the last commit. 
  -> git pull: pulls changes from repository and merges with master.
  -> git fetch <remote> <branch>: grabs the <branch> from remote into a local branch called FETCH_HEAD
  -> git rebase: apply current changes to a branch (merge with branch).
  -> instead of pull: use git fetch origin master + git rebase FETCH_HEAD; safer, easier to manage conflicts etc.
  -> git reset head: resets branch to lastest commit on master (discarding all local changes!)
  -> git reset head~2: moves the branch in the state it was in 2 commits in the past (removing changes).
  -> git reset <commit_id>: resets branch to specific commit.
  -> git cherry-pick <commit_id> <branch>: grabs changes form specific commit, or specific branch and aplies them to current branch.
  -> git push <remote> <branch>: push current commited changes to the remote server.
  -> git log: history log of all commits!
  -> tip: git log --pretty=oneline : grabs a summary of them and displays the log in a neat format!
  
  typical workflow:
    -> git fetch origin master (grabs latest state of master branch)
    -> git rebase FETCH_HEAD (applies your changes on top of that - merging inside your current local branch)
    -> add / modify / remove files locally
    -> git add / git rm...
    -> git commit -m "commit message"
    -> git push origin master
  
  use git status to understand your current changes and what is done already / needs doing etc.
  
  Feel free to use this test repo to try out whatever commands you need!
