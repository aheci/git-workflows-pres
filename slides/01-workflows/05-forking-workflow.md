---
title: Forking Workflow
layout: Center
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
<div class="workflow-image">
  <img src="https://www.atlassian.com/dam/jcr:5c0941ff-a8b5-435b-a092-2167705f1e97/01.svg" />
</div>

- Every developer has a server-side repository
- Each contributor has 2 Git repositories - one private local one and one public server-side one
- Only the project maintainer can push to the official repository (accept commits without giving write access)
- Still create a feature branch every time you start a new feature