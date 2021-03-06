# Outline

1. Installation
   * Setup github account
   * [`http://git-scm.com/downloads`](http://git-scm.com/downloads)
   * Windows installation: Accept all defaults
1. Setup
   * Identity 
     - `$ git config --global user.name "Name"`
     - `$ git config --global user.email user@example.com`
   * Configuration Files `~/.gitconfig`
1. Cloning
   * `git clone http://github.com/joshuavial/git-workshop.git`
   * `cd git-workshop`
1. Create a feature branch
   * `git checkout -b my-feature`
1. Modify files 
1. Check the status
   * `git status`
1. Stage files
   * `git add index.html`
   * `git add style.css`
   * `git status`
1. Commit staged changes
   * `git commit -m 'my message`
1. Check the log
    * `git log`
1. Merge into master
    * `git checkout master`
    * `git merge my-feature`
1. Demonstration of push
1. Create a release branch
    * `git checkout -b release-1`
    * Modify branch with bugfixes and commit to release
1. Merge into master and dev
    * `git checkout master`
    * `git merge release-1`
    * `git push origin master`
    * `git checkout dev`
    * `git merge release-1`
    * `git push origin dev`
1. Tagging the release
    * `git checkout master`
    * `git tag 1.0`
1. Merge conflict resolution
    * Git will create a new commit when merge conflicts occur
    * Any files that now have merge conflicts will have resolution markers in them
    * Git will also add local, remote, and base versions of the file for you to diff against
    * When you are satisfied with the merge run
      - `$ git add <filename>`
      - `$ git commit`
    * The mergetool may come in handy
      - `$ git config --global merge.tool vimdiff`
      - `$ git mergetool`
1. Other concepts
    * `git help`
    * Creating new repositories with `git init`
    * Ignoring files with `.gitignore`
    * `git stash` and `git stash pop`
    * Adding/removing remote repositories
1. Resources
    * Pro Git (Book)
      - Free online [`http://git-scm.com/book`](http://git-scm.com/book)
    * Try git online
      - [`http://try.github.io/levels/1/challenges/1`](http://try.github.io/levels/1/challenges/1)
    * Git Immersion
      - [`http://gitimmersion.com/lab_01.html`](http://gitimmersion.com/lab_01.html)
    * Check out the presentation
      - [`http://brian-jesse.com/gittalk`](http://brian-jesse.com/gittalk)
    * Git Branching Model
      - [`http://nvie.com/posts/a-successful-git-branching-model/`](http://nvie.com/posts/a-successful-git-branching-model/)

