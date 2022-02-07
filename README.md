### ds219sp2022 Feb 9, 2022

#### This is a repository for students of DS 219

##### Fork then clone this repository

```shell
# fork first
git clone git@github.com:yourname/ds219sp2022.git
cd ds219sp2022
git remote add upstream git@github.com:sallyom/ds219sp2022.git

```

##### Create a new branch for new work

```shell
git checkout -b my-new-branch
```

###### Continually keep your local working branch up to date with upstream main branch

```shell
git fetch --all
git rebase upstream/main
# the above ensures your local working branch is current with latest changes in upstream main branch
```
###### Add a file to your local branch

(and watch [History of Kubernetes Part 1](https://youtu.be/BE77h7dmoQU)

```shell
# Create a file in this repository with the name "your-name-date"
# In this file, answer question 1: "Did you watch the 'History of Kubernetes Part I' video?"
# In thid file, answer question 2: "Did you find the video interesting? Why or why not?"
# In this file, answer question 3: "What editor did you use to write this file?"

git add .
git commit -m "your-name-date"
```

##### When you are ready to push your local working branch to your GH repository

```shell
git push origin my-new-branch
```

##### Submit a Pull Request to the upstream repository

```shell
This you will most likely do from the GitHub site
```

##### After the initial push of your branch to GH, you will have to use `--force-with-lease` for any push.

Read [here](https://blog.developer.atlassian.com/force-with-lease/) for more information about force pushing.

```shell
git push --force-with-lease origin my-new-branch
```

##### Continually keep your local and remote `main` branch up to date with upstream main branch

```shell
git fetch --all
git rebase upstream/main
git push --force-with-lease origin my-new-branch
```
