---
title: Namespacing Branches
style: |
  .fa-question {
    color: #E40046;
  }
---

---

"Special" branches are branches that are reserved for specific purposes.  It is usually hurts the entire team when they are not used as intended.

<div class="callout warning">

  <i class="fa fa-info-circle" aria-hidden="true"></i> **That's Smelly! Signs you have a problem**
  
  Special branches should never be *behind* master.  When we update master we are responsible for updating the other special branches as well.
</div>

On the marketing sites we have:
- `master` this branch is sacred and is reserved for code that has been tested, approved by QA, and cleared for release by stakeholders.  There should be zero risk in deploying this branch.
- `hko-[environment]` branches
  1. These branches are reserved for code compiled by grunt tasks
  2. Our Heroku environments "listen" to these branches and automatically rebuild the sites when updates are made to them
  3. files should never be directly edited in these branches <i class="fa fa-question fa-lg"></i> 
- `core-[who]` branches
  1. These branches are to aggregate types of features (described as the develop branch in the workflows we covered)
  2. You should avoid working in these branches directly and instead submit a PR the one that meets your needs
    - `core-seo` kept in sync with master and is a place for the SEO team to make content and meta data updates that can go live independent of any other features currently being developed
    - `core-dev` this is our develop branch.  As we work on features to be released at the end of a sprint we add them to this branch as they are ready via a Pull Request.  Deploying to the QA environment happens from here.  <i class="fa fa-question fa-lg"></i>  Should never be behind master.  <i class="fa fa-question fa-lg"></i> 
- `global-[what]` branches
  - Right now this consists only of `global-push` and is reserved for receiving updates from the global framework.  
  - This is a pull only branch - we don't edit files directly in this branch or submit PRs to these branches. 
  - If you have a need to work in these files it is done through the UX Frontend Framework.  <i class="fa fa-question fa-lg"></i> 