# Git exercise project

this project will be used for series git exercise

# Bundle 4

## Exercise 1
- Checkout the `main` branch
- Create a new repository on github
- Using git remote add the repo to your project as second remote named `git-copy`
- Make a new changes on the home page
- Commit the changes
- Push the changes to the both remotes. the `origin` and `git-copy`

```bash
git checkout main get in main
creating new repo on github called git-exercises-clone
git remote add git-copy https://github.com/Shema486/git-exercise-clone.git  to make clone of git-exercise
git commit -m "feature added to home"
git push origin
git push git-copy
git remote remove git-copy
```
### Exercise 2
- Checkout a new branch named `ft/footer`
- Add some changes to the branch and commit them
- Add more changes again to the branch and create a second commit
- Push and create a new PR for the branch
- Checkout the `main` branch again
- From there create a new branch named `ft/squashing`
- Using git merge squash, squash the changes on the `ft/footer` branch
- Commit the changes with a different commit message such as `footer changes squashing`
- Push the changes and create a PR
```bash
git checkout -b ft/footer
adding some changes to branch
more changes and commit
git push origin ft/footer and pull request
git checkout main branch
git checkout -b ft/squashing
git merge squash

```