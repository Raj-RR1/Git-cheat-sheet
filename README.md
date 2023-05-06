# Git-cheat-sheet
Commonly used git commands

1. Delete branch locally as well as in remote.
- Checkout to a different branch -> **git checkout <branch-name>**
- Delete branch locally -> **git branch -d <branch-name>**
- Delete branch on remote -> **git push <remote-name> --delete <branch-name>**

1. To check if a branch in local is sync with remote branch
- Git fetch
- Checkout to branch you want to check if it is in sync -> **git checkout <branch-name>**
- See commits that are on remote but not on local -> **git log HEAD..origin/<branch-name>**
- Check status of local branch compared to remote -> **git status**

1. Apply remote changes to local branch
- Checkout to the branch you want to apply changes -> **git checkout <branch-name>**
- **git merge origin/<branch-name>**
- Verify that local branch is up to date with remote- **git log OR git status**
1. Bring branch that is present in remote to local.
- **git fetch**
- **git checkout -b <branch-name> origin/<branch-name>**