---
title: Naming Feature Branches
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
Why does it matter how we name our feature branches?

Think about this scenario:

> Cody & Chris are working together on an update to the program page template that fixes a bug in production.  They're almost done but go to lunch and eat Pho, run from the table holding their stomachs and we don't hear from them again for three days?
  
Flo & Shaun are on their own & stakeholders are standing at their desks demanding to know why this fix isn't live yet.  They each have their own deliverables for this sprint and haven't been in touch with the progress on this issue.

What are the consequences of this branch being named `cody-branch-50` and the project containing 50 other similarly named branches?

<div class="workflow-image">
<img src="./angry-emoji.jpeg" /> x2
</div>