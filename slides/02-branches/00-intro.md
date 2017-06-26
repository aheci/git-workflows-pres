---
title: Keeping Repos Organized
chapter: Branches
---
3 out of 4 of the workflows we just covered use a branching strategy requiring a branch for each feature.  With all those branches, how do we keep things organized?

Branch names become very important in these workflows and should not be overlooked.  Done right, branch names should serve as a **brief** summary of the changes made within the branch.

If we have more than just master & develop for "special" branches - we should namespace & document them

We must keep the playground clean.  After you merge a PR - please be kind and press the delete branch button.  This helps everyone understand what is currently in progress and what is complete.


<div class="callout warning">

**Fooled Me! Location matters**

When creating a branch it *matters* where you are in your repo.  

```
on branch `core-dev`
git checkout -b hotfix-must-go-live-now
```

This branch will include all commits from the core-dev branch you are currently in.

```
on branch `master`
git checkout -b hotfix-must-go-live-now
```

This branch will include all commits from only the master branch that you are currently in.

*Which one do we want?*

</div>