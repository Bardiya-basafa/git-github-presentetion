# git-github-presentetion
# working with branches
+ what is branch master 
+ what is head
+ some branching and concept of branch
+ detached head
+ git checkout and switch
```
    git branch
    git branch <branch_name>
    git switch <branch_name>
    git switch -c <branch_name>
    git branch -v(verbose : more information on branch)
    git switch - (back to last branch)
    git checkout <commit_hash>
    git checkout <branch_name>
    cd ./.git
    cat HEAD. cat refs/heads
```

# vscode source control
+ what is it
+ some features of it
+ how to work with
+ benefits of it

# merging
+ what is merging
+ fast forward merge
+ merge conflicts
+ resolving merge conflicts
+ deleting branches
```
    git switch <branch_name>
    git merge main (fast forwad)
    git merge main (merge commit : merge conflicts)
    git branch -d <branch_name>
    git brancg -D(force delte) <branch_name> 
```


# stashing
+ what is stashing
+ why we need stash
+ stash save
+ stash list, pop, drop, apply, -u, clear
```
git stash save <stash_name>
git stash list
git stash pop
git stash apply
git stash push
git stash drop
git stash -u
git stash clear
```

# undoing
+ power of git checkout
+ detached head
+ how head actualy works
+ checkout old commits
+ git resotre
+ git reset hard and soft
+ git revert and its benefits
```
git log --all --graph
git checkout <history_commit_hash>
git switch -c (at a history commit)
git checkout HEAD~1
git checkout HEAD <file>
git checkout -- <file>
git restore <file/directory>
git restore --source HEAD~1 <file>
git resotre --staged <file>
git reset <commit_hash> (remove commits after)
git reset --hard <commit_hash> (remove all the changes and files)
git revert <commit_hash> (makes a new commit for changes)
```

# github basic
+ some github basics how clouds works
+ ssh on github
+ remote
+ pushing
+ workflow of intracting with git and github
```
git clone <url>
ssh -T git@github.com
git remote -v
git remote add <name> <url>
git remote remove <name>
git remote rename
git push <remote> <branch>
```

# fetching and pulling
+ what is remote tracking branch
+ checking out remote tracking branch and comparing
+ git fetch
+ fetch remote branch
+ git pull
+ compare pull and fetch
+ pull merging
+ diverion branch and merge conflicts
+ fetch merge and pull
+ working with both and demo some merge conflits on diversion branch
```
git branch -r
git switch <remote_tracking_branch>
git statusmain
git fetch <remote>
git fetch <remote> <branch>
git pull = git fetch + git merge
git pull <remote> <branch>
git pull (with merge conflict)
git fetch origin <branch> (wtih merge conflict)
git merge <branch> <origin/branch> (merge conflict)
(diversion branching)
```

# some other things on github
+ public vs private
+ what is collaboration
+ github pages


# github collaborations
+ workflow of centralized branching
+ feature branching
+ what is pull request
+ why pull request
+ some demo pull requests
+ forking
+ forking then cloning
+ adding remote (upstream) from base repo
+ pulling from base repo
+ pushing to ourself repo
+ pull request to the base repo

# rebasing
+ what is rebasing
+ scenario of a rebase
+ why rebasing
+ rebase as a cleaning up tool
+ rebase is very dangrous
```
git branch <some_feature>
git commits
git merges main
git switch <some_feature>
git rebase main (resove conflicts)
git rebase -i HEAD~3 (re writting history)
```

# CI/CD basics
+ why we need ci/cd
+ what it actually does
+ what are the platforms
+ what we can actually do in piplines
+ what is github actions
+ some action demo
+ familarity with actions
  







