---
title: Rebase Quick Tips
style: |
  .exerslide-slide .Center-wrapper {
    text-align: left;
  }
  .exerslide-slide h1 {
    text-align: center;
  }
  h4 {
    font-weight: bold;
  }
  .workflow-image {
    width: 100%;
    text-align: center;
  }
  .workflow-image img {
    height: 200px;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 50px;
  }
---
---

- `git rebase [branch]` is similar to `git pull [branch]` but without the annoying commit message
- `git squash` is like saying take these 18 commits and smush them into 1
- `git rebase -i [hash *or* branch]` lets us perform both tasks at once