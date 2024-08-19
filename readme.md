# Git exercise project

this project will be used for series git exercise

## Bundle 2

### Exercise 2
- Checkout your `main` branch and pull the latest changes
- Create a new branch named `ft/service-redesign`
- Add new changes to the `service.html` page
- commit and push them
- create a new PR for your changes
- go back to your `main` branch and add again new changes to your `service.html` page, you can add different changes but make sure to affect the same part(line of code) as you did in the other PR
- Commit and push those changes
- Using git revert, revert the changes of the last commit of the `ft/team-page` branch. (use the commit hash you copied earlier)
- Push the changes and create a new PR


#### WORKOUT
```bash  
eligr@Shema MINGW64 ~/git-exercises (main)
$ git checkout -b ft/service-redesign 
Switched to a new branch 'ft/service-redesign



eligr@Shema MINGW64 ~/git-exercises (ft/service-redesign)
<<<<<<< HEAD
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page
=======
$ git status
On branch ft/service-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   readme.md
        modified:   service.html

eligr@Shema MINGW64 ~/git-exercises (ft/service-redesign)
$  git push --set-upstream origin ft/service-redesign
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.04 KiB | 533.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Shema486/git-exercises/pull/new/ft/service-redesign
remote:
To https://github.com/Shema486/git-exercises.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
>>>>>>> 446750f (hRevert " cherry-pick practice")


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
eligr@Shema MINGW64 ~/git-exercises (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is ahead of 'origin/ft/team-page' by 1 commit.
  (use "git push" to publish your local commits)

eligr@Shema MINGW64 ~/git-exercises (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

eligr@Shema MINGW64 ~/git-exercises (main)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is ahead of 'origin/ft/team-page' by 1 commit.
  (use "git push" to publish your local commits)

  eligr@Shema MINGW64 ~/git-exercises (ft/team-page)

eligr@Shema MINGW64 ~/git-exercises (ft/service-redesign)
$  git push --set-upstream origin ft/service-redesign
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.04 KiB | 533.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Shema486/git-exercises/pull/new/ft/service-redesign
remote:
To https://github.com/Shema486/git-exercises.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.



eligr@Shema MINGW64 ~/git-exercises (ft/service-redesign)

$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.


```

