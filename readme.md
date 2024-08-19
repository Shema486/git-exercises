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


```