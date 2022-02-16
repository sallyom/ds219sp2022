### ds219sp2022 Feb 16, 2022

This is a branch to report attendance Spring 2022 DS 219

#### Follow [README.md](https://github.com/sallyom/ds219sp2022#readme)

Each week, when you arrive to class, do the following:
* Create a file with the name "your-name-date"
* In this file:
    * answer question: "What editor did you use to write this file?"

```shell
# If working from a terminal
git checkout -b attendance-feb-16
<nano, gedit, vim> Feb-16/sally-omalley-feb-16.md
    # Add line to this file with "I used <editor> to create this file."
    # Add anything else you want (questions? comments? nothing?) 
git add .
git commit -m "your-name-date"
git push origin attendance-feb-16

# If working from GitHub site, do the equivalent of the above
```

#### Submit a Pull Request to the upstream repository main branch

```
This you will most likely do from the GitHub site
```

#### Continually keep your local `main` and remote `main` branch up to date with upstream main branch

```shell
git checkout main
git fetch --all
git rebase upstream/main
git push origin main
```
