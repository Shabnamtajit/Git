                                                                Git

Git is a distributed version control framework that is free and open source.
It is used for project collaboration and history exploration.

Features of Git:

  1. Fully distributed VCS
  2. Data Integrity And Security
  3. Supports Non-linear Development
  4. Branching
  5. Lightweight and Fast

Perfect Commit Message:

  1. Subject -> consise summary of what happened
  2. Body-> a) different than before
            b) Reason for change
            c) Anything particularly remarkable

Working of Git:
1. Working tree - contains files that we are working on 
2. Staging area - contains all added files/new/changed to the next commit
3. Repository.  - it is a project's database.

Every files goes through 3 stages:
   1. Modified
   2. Staged
   3. Committed

Branching strategies:
   1. Written convention
   2. Integration: few branches, relatively small commits, high quality testing
   3. State , release and feature branches
        a) long Running branch: exist complete lifetime of project
                                Often they mirror "stages" dev life cycle
                                No direct commits
        b) Short lived branch : for new feature, bug fixes, refractories , experiments
                                Will be deleted after integration ( merge/rebase)

Examples:
1. GitHub Flow: very simple, lean
                Has only 1 long- run branch( main )+ feature branches
                
2. GitFlow: more structures, more rules
            Long-running:"main"+ develop
            Short-lived: features, releases,hotfixes

PULL REQUEST:

   It invites reviewers to provide feedback before merging
   Contributing code to other Repository

FORK:

   It is creating fork of original Repository and where we can make changes and suggests those changes to be included via a pull request.
   

MERGE CONFLICTS:

   Conflicts occur when integrating commits from different sources.
   (Like..Merge, rebase, clurry-pick, Stash apply,pull request)

How to solve a conflict: clean up the file:

                       MERGE.                              Vs.                                                   REBASE

   1. Merge lets you merge different branches.                                       Rebase allows to integrate the changes from one branch to another.
   2. Shows complete history of commit merging .                                     Rebase logs are Linear
   3. All commits are combined into a single master branch.                          Same number of commits are added to master branch.
   4. Best used when target branch is to be shared.                                  Best used when target branch is private.
   5. Preserve history.                                                              Rewrites history.

NOTES:

  a) Do not use Rebase on commits that have already pushed/shared on remote repository.
  
  b) Instead use it for cleaning up local commit history before merging it into shared team branch.
