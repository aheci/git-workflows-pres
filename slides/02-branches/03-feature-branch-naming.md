---
title: Feature Branch Naming
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
Name that Branch!

> Dev Two & Dev Three are working together on an update to the program page template that fixes a bug in production.  They're almost done but go to lunch and eat Pho, run from the table holding their stomachs and we don't hear from them again for three days?

Based on this limited information, a better name for this branch would've been `hotfix-program-template-bug`
  
<div class="callout primary">

<i class="fa fa-info-circle" aria-hidden="true"></i> Bonus Points

If our projects are organized in a system that provides ticket, task, or issue numbers - we should use that number in our branch name for easy reference.

```
git checkout -b `#78478-hotfix-program-template-bug`
```

</div>