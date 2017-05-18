# Learn Git Lab

1. Create a fork of the [learn-git repository](https://github.com/sf-wdi-27-28/learn-git) by clicking "Fork" on the top right.



2. You'll see a screen like this while GitHub is forking the repo. Forking creates a copy of the original repo on your own GitHub account.



3. Now you have your own copy of the repo! Copy the "clone URL" from the top.



4. Use the "clone URL" to clone the repo onto your local machine. Make sure you're in your `~/dev` directory before you clone!

  ```zsh
  ➜  cd ~/dev
  ➜  git clone <clone-url>
  ```

5. Change directories into the repo you just cloned (in this example, `learn-git`).

  ```zsh
  ➜  cd learn-git
  ```

6. Open this project in Atom.

  ```zsh
  atom .
  ```

1. Back in Atom, open `index.html`. In the `<body>` tags, create an `<h1>` tag with your name and add a gif of your liking in an `<img>` tag. "Copy Image Address" from [giphy.com](http://giphy.com/).

6. Now that you've changed the repo, it's time to commit your changes. Back in your terminal, type

  ```zsh
  ➜  git status
  ```
  This shows you the files that have been modified, created, or deleted. Notice that they are listed as `untracked`.

1. Now you're ready to `add` your changes. Type
  ```
  ➜  git add .
  ```
  Then `git status`. Notice that your new file has gone from `untracked` to `Changes to be committed`.

1. Next step is committing. Type

  ```
  ➜  git commit -m "modifying index.html"
  ```
  Then `git status`. Notice that the new status is `Your branch is ahead of 'origin/master' by 1 commit.`. This indicates that your the version of the repo on your computer (aka the __local__ version) includes your changes but the version hosted by GitHub (aka the __remote__ version) does not.

1. To get your changes on to the remote version of the repo, type

  ```
  ➜  git push origin master
  ```
  Now `git status` will tell you that `Your branch is up-to-date with 'origin/master'.` __!!!__

7. Once you're done with the assignment and have committed and pushed ALL of your changes to GitHub, it's time to make a pull request back to the original repo. Go to your forked copy of the repo on GitHub, and click the "Pull Request" button.


8. GitHub takes you to a new view and asks if you want to create the pull request. Click the green button, and that's it - you've now created a pull request to submit this lab!


1. Repeat! Add some new content to your file and repeat this Git flow.
