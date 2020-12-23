# gitcommands
Playbook for git commands

### Git Commands:
1. Create new local repo: `git init`
1. Add files to local repo: `git add .` (don't forget the `"."` at the end)
1. Check on git status: `git status`
1. Commit to local repo: `git commit -m "commit message here"`
1. Add remote origin repo: `git remote add origin REPO_URL`
1. Push to remote repo: `git push`
1. List git configurations: `git config --list`
1. Pull code from remote repo to local repo: `git pull`
1. Change remote origin repo: `git remote set-url CHANGED_REPO_URL`
1. Check remote repo: `git remote -v`
1. Move branch from master to main: `git branch -m master main`
    * We use `branch -m` to move the branch locally instead of creating a new one with `checkout -b` like you might be used to.
    * https://stackoverflow.com/questions/64249491/difference-between-main-branch-and-master-branch-in-github
    * https://jarv.is/notes/github-rename-master/
1. Set the new branch as the local repo default:  `git push -u origin main`
    * The `push -u` sets the new branch as the local default at the same time
1. Local head points to new branch on remote repo: `git remote set-head origin main`
    * ensures our local HEAD points to our new branch on GitHub.
1. Check remote repo branch: `git branch -r`
1. Delete the old master branch on GitHub (remote repo): `git push origin --delete master`
    * We used -m (move) to rename the master branch locally, but GitHub will still have two identical branches at this point (as you saw in the previous step). 
    * Deleting it can be a little nerve-racking, so poke around your repository on GitHub and make sure your new branch is there and the commit history is correct.
1. Set git credentials using helper: `git config --global credential.helper store` 
1. Alternate way of setting remote repo: `git push --set-upstream origin main`
    * https://stackoverflow.com/questions/37770467/why-do-i-have-to-git-push-set-upstream-origin-branch
    * https://devconnected.com/how-to-set-upstream-branch-on-git/

### Windows CLI Commands:
1. Create directory: `mkdir folder_name`
1. Open/create file in Notepad++: `start notepad++ file_name.txt`
1. Open/create file in Notepad++ within folder: `start notepad++ folder_name/file_name.txt`
