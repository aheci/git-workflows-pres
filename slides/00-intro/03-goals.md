---
title: Goals
style: |
  .workflow-image {
    width: 100%;
    text-align: center;
  }
  .workflow-image img {
    height: 300px;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 50px;
  }
---
After this presentation I hope we have a better understanding of our GitHub workflow & why each of these commitments are important:
- Don't be a bus factor: we will use sensible branch names & commit messages
- Keep the playground clean: If you merge the branch, you delete the branch
- Let your commit speak for itself - One message per feature before merged
- Isolate changes - one feature per branch
- Master is the bible - this is always a representation of what is live NOW.  Deploying it should never introduce any unexpected features
- Friends don't let friends overwrite each others code - QA builds are done from core-dev

<div class="workflow-image">
<img src="./pinky-promise.jpg" />
</div>