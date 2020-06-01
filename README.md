## Johann's personal road to the utmost most wonderful git mastery
## First steps

### download git
```
git init # initialise git
```

### fork my repository to your github account (create one if you don't have one yet)
```
git clone https://github.com/<johann-account>/cciwr.git # clone forked repository from your github (use SSH instead of HTTPS -> readup on this)
git remote add felix git@github.com:derpyninja/cciwr.git # set my repository as a new remote
git remote -v
```

## Common workflow
```
git fetch origin master # see if there are any changes, doesn't download anything yet (if other party changes stuff)
git pull origin master # update the local state to the latest remote master state (pull changes into local directory)
```

### ... now you do some work on your local files and then ...
```
git status # check for local changes
git add . # add untracked files and stage them
git commit -m "message" # commit changes in local repository
git push origin master # push current HEAD to YOUR remote master branch (push to my github and then create pullrequest)
git push felix master # push current HEAD to MY remote master branch (only if administrator, then push directly into master)
```

## Additional steps to check if everything now works
### I've now turned off network iv6 by "networksetup -setv6off Wi-Fi", can be turned back on by "networksetup -setv6automatic Wi-Fi"
```
```