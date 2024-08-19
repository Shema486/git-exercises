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


eligr@Shema MINGW64 ~/git-exercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.


```
## Bundle 3 ### Exercise 2
- Create new branch from the `ft/faq-page` branch named `ft/home-page-redesign`
- Go back to the `main` branch and make some changes there
- Commit and push them
- go back to the `ft/home-page-redesign` branch
- Using git rebase, rebase your branch to `main`
- Add changes to the home page and commit push them
- Create a PR for the changes.
