# Git exercise project

this project will be used for series git exercise

## Exercise 1
```bash
Exercise 1

- Create a project & initialize git
- Rename your main branch from `master` to `main`
- Make changes to the project (add files, rename them or edit them)
- Stage your changes and commit them
- Create a github repo and connect it with your project
- Push your changes to github
- Create a new branch `dev`
- From `dev` create another branch `test`
- Go back to the `dev` branch and delete the `test` branch


eligr@Shema MINGW64 ~/git-exercises (master)
$ git branch -m main

eligr@Shema MINGW64 ~/git-exercises (main)
$ git status
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)

eligr@Shema MINGW64 ~/git-exercises (main)
$ git add readme.md

eligr@Shema MINGW64 ~/git-exercises (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   readme.md


eligr@Shema MINGW64 ~/git-exercises (main)
$ git commit -m "init project"
[main (root-commit) 95ab917] init project
 1 file changed, 3 insertions(+)
 create mode 100644 readme.md

eligr@Shema MINGW64 ~/git-exercises (main)
$ git remote add origin https://github.com/Shema486/git-exercises.git

eligr@Shema MINGW64 ~/git-exercises (main)
$ git status
On branch main
nothing to commit, working tree clean

eligr@Shema MINGW64 ~/git-exercises (main)
$  git push --set-upstream origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 268 bytes | 134.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Shema486/git-exercises.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

eligr@Shema MINGW64 ~/git-exercises (main)
$ git checkout -b dev
Switched to a new branch 'dev'

eligr@Shema MINGW64 ~/git-exercises (dev)
$ git status
On branch dev
nothing to commit, working tree clean

eligr@Shema MINGW64 ~/git-exercises (dev)
$ git status
On branch dev
nothing to commit, working tree clean

eligr@Shema MINGW64 ~/git-exercises (dev)
$ git push origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Shema486/git-exercises/pull/new/dev
remote:
To https://github.com/Shema486/git-exercises.git
 * [new branch]      dev -> dev

eligr@Shema MINGW64 ~/git-exercises (dev)
$ git checkout -b test
Switched to a new branch 'test'

eligr@Shema MINGW64 ~/git-exercises (test)
$ git status
On branch test
nothing to commit, working tree clean

eligr@Shema MINGW64 ~/git-exercises (test)
$ git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/Shema486/git-exercises/pull/new/test
remote:
To https://github.com/Shema486/git-exercises.git
 * [new branch]      test -> test

eligr@Shema MINGW64 ~/git-exercises (test)
$ git checkout dev
Switched to branch 'dev'

eligr@Shema MINGW64 ~/git-exercises (dev)
$ git branch -D test
Deleted branch test (was 95ab917).

eligr@Shema MINGW64 ~/git-exercises (dev)
$ git push origin --delete test
To https://github.com/Shema486/git-exercises.git
 - [deleted]         test

eligr@Shema MINGW64 ~/git-exercises (dev)
$ git checkout -b shema
Switched to a new branch 'shema'

eligr@Shema MINGW64 ~/git-exercises (shema)
$ git status
On branch shema
nothing to commit, working tree clean

```