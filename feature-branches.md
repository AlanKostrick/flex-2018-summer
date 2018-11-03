# Feature Branches

We will be using feature branches to build out all of our content for the final project. All feature branches will be verified and
merged to master via pull requests. 

## Working rules
- Do not code on master on your local machine but if you find yourself in this position we can fix it
  - `git stash` will take all of your changes on master and remember them
  - `git checkout -b new-branch` then `git stash apply` will take these changes you had on master and place them on your new branch
- Do not add/commit/push to the master branch 

## The process
- Make a feature branch for every "feature" you plan on adding into your application
- Since we work in iterations, these should be todos from your trello cards for a particular sprint
- Name your feature branch to match the feature you are building
  - For example `git checkout -b account-and-bank-build` may be a branch that a dev creates to test and build these entities out
  - You can `add commit push` to this branch as much as you would like
  - When ready, submit the pull request on git hub
  - A teammate will verify the pull request(pr) and merge to master on git hub
  - Entire team can do a `git pull` to pull these changes into master
  
  ## Navigating branches
  - `git checkout master` allows you to leave a feature branch and go back to master
  - bash will warn you to  `add and commit` your changes before it will let you leave a branch!
  - `git checkout branch-name` allows you to move from master or one branch to another...again, bash will make sure all changes
  are stored before letting you out of a branch
  
  ## Tips
  - Keep it very very simple. No more no less than what is above. There is no need to do any rebasing or to get crazy with the
  endless commands that googling bash issues could lead you to 
  - COMMUNICATE COMMUNICATE COMMUNICATE!
    - Let team members know if you put in a PR
    - Let team members know when you merged a PR and it is good to pull to master
    - Work on separate parts of the app...definitely ensure you are in different files to avoid major merge conflicts
   - Be sure to avoid any manual uploads to Git Hub, these most likely will unintentionally go to master 
   
