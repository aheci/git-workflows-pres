---
title: Example - Rewriting History
---

---

```
git checkout core-dev
git pull origin core-dev
git checkout #123-new-feature
git rebase core-dev
git log
git rebase -i [copied-SHA1]
git push -f

```
1. `git rebase core-dev` - This puts all of your commits on top of core-dev without adding an additional merge message to your commit history
2. `git log` - This shows you a log of the commit history and the hashes for each commit message.  You are looking for the last commit to the core-dev branch.  You will then copy the hash for that commit
3. `git rebase -i [copied-hash]` - Tells git you want to squash the commit messages that come after the hash you selected
    - Your preferred text editor will launch & show you all the commits that have been made on top of the hash you selected
    - You write "pick" at the beginning of the line for the commit you want to roll all other commits into
    - You write "squash" at the beginning of the line for the commits you want to no longer see broken out individually
    - Save your changes
    - Close the editor!
    - Another editor will open asking you to decide what your commit message will be.  Delete all of the old ones and write a new one that describes the code and includes a ticket number `[#123] New Feature`
    - Save & close again
4. `git push -f` If you do not force push your changes will be rejected because the remote branch has a history of individual commits that it can no longer find in your local branch (getting rid of them was our goal)