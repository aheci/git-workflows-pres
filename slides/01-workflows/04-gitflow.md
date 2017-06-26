---
title: Gitflow Workflow
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
  <img src="https://www.atlassian.com/dam/jcr:e3bd4199-27ac-4bac-a5d2-3ff0fdb112d3/01.svg" />
</div>

- One central repository
- Master represents what's live right now
- Develop represents a group of features that are being aggregated to go live next
- Create a feature branch every time you start a new feature
- ONE feature per branch
  - PR to master for changes that need to go live in isolation
  - PR to develop for changes that need to be QA'd along with other features for the next release