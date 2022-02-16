### ds219sp2022 Feb 9, 2022

This is a repository for students in Spring 2022 DS 219

#### Be sure you've set your text editor in your local git config

This only has to be run once, it's a global git setting that will apply
to all of your local github repositories. In the below example,
[atom](https://blog.atom.io/2014/12/10/a-windows-installer-and-updater.html) is set.

`atom` is a common and easy-to-use editor, but you can set any editor you prefer.

```shell
git config --global core.editor "atom"
```

#### Fork then clone this repository

```shell
# fork first
git clone git@github.com:yourname/ds219sp2022.git
cd ds219sp2022
git remote add upstream git@github.com:sallyom/ds219sp2022.git
```

#### Create a new branch for new work

```shell
git checkout -b my-new-branch
```

#### Continually keep your local working branch up to date with upstream main branch

```shell
# this ensures your local working branch is current with latest upstream main branch
git fetch --all
git rebase upstream/main
```

#### Add a file to your local branch

(and watch [History of Kubernetes Part 1](https://youtu.be/BE77h7dmoQU))

```shell
# Create a file in this repository with the name "your-name-date"
# In this file:
#     answer question 1: "Did you watch the 'History of Kubernetes Part I' video?"
#     answer question 2: "Did you find the video interesting? Why or why not?"
#     answer question 3: "What editor did you use to write this file?"

git add .
git commit -m "your-name-date"
```

#### When you are ready to push your local working branch to your GH repository

```shell
git push origin my-new-branch
```

#### Submit a Pull Request to the upstream repository

```
This you will most likely do from the GitHub site
```

#### After the initial push of your branch to GH, you will have to use `--force-with-lease` for any push.

Read [here](https://blog.developer.atlassian.com/force-with-lease/) for more information about force pushing.

```shell
git push --force-with-lease origin my-new-branch
```

#### Continually keep your local and remote `main` branch up to date with upstream main branch

```shell
git fetch --all
git rebase upstream/main
git push --force-with-lease origin my-new-branch
```

#### To get back to your main branch

You won't be able to check out a branch unless the branch you are currently working
in is clean, ie, you've commited all changes locally

```shell
git checkout main
```
