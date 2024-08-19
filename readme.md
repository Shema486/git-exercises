# Git exercise project

this project will be used for series git exercise

## Bundle 3

### Exercise 1
- Create a new branch named `ft/team-page`
- Create a new html page named `team.html` and add some changes
- commit and push those changes
- Create a new PR for the changes
- Go back to `main` branch (checkout the `main` branch)
- Create new branch named `ft/contact-page`
- Go back to the `ft/team-page`
- With the help of git log look for the last commit and copy its hash
- Checkout again `ft/contact-page` using git cherry-pick get the changes from the last commit on the `ft/team-page` branch.
- Add new changes for the contact page and commit, push them
- Create a new PR for the contact page
- From the `ft/contact-page` branch create a new branch called `ft/faq-page`
- Create a new `faq.html` page and add some changes there
- Commit and push those changes
- Now go back to the github PR you had created for the `ft/service-redesign`branch, you will then see that you have conflicts with the `main` branch
- In your project checkout the `ft/service-redesign`branch
- Compare the `ft/service-redesign`with the `main` branch using git diff and observe the changes
- Using git merge, merge the `main` branch with `ft/service-redesign` branch and commit and push you changes again

#### WORKOUT  
```bash
eligr@Shema MINGW64 ~/git-exercises (main)
$ git checkout -b ft/service-redesign 
Switched to a new branch 'ft/service-redesign


eligr@Shema MINGW64 ~/git-exercises (ft/service-redesign)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'


eligr@Shema MINGW64 ~/git-exercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```
## cherry-pick
```bash
$ git cherry-pick a7294891b4f077db26990e242abad3d58d8a61d2
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
error: could not apply a729489... new change in team
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git cherry-pick --continue".
hint: You can instead skip this commit with "git cherry-pick --skip".
hint: To abort and get back to the state before "git cherry-pick",
hint: run "git cherry-pick --abort".
hint: Disable this message with "git config advice.mergeConflict false"

eligr@Shema MINGW64 ~/git-exercises (ft/contact-page|CHERRY-PICKING)
$ git status
On branch ft/contact-page
You are currently cherry-picking commit a729489.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Changes to be committed:
        modified:   readme.md
        new file:   team.html


eligr@Shema MINGW64 ~/git-exercises (ft/contact-page|CHERRY-PICKING)
$ git add contact.html

eligr@Shema MINGW64 ~/git-exercises (ft/contact-page|CHERRY-PICKING)
$ git status
On branch ft/contact-page
You are currently cherry-picking commit a729489.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Changes to be committed:
        new file:   contact.html
        modified:   readme.md
        new file:   team.html
```