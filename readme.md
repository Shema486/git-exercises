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
- Using git revert, revert the changes of the last commit of the `ft/team-page` branch. (use the commit hash you copied earlier)
- Push the changes and create a new PR

## WORKOUT
```bash
eligr@Shema MINGW64 ~/git-exercises (ft/service-redesign)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

eligr@Shema MINGW64 ~/git-exercises (ft/team-page)
$ git add --all

eligr@Shema MINGW64 ~/git-exercises (ft/team-page)
$ git status
On branch ft/team-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   readme.md
        new file:   team.html


eligr@Shema MINGW64 ~/git-exercises (ft/team-page)
$ git commit -m "new change in team"
[ft/team-page a729489] new change in team
 2 files changed, 38 insertions(+), 41 deletions(-)
 create mode 100644 team.html


```