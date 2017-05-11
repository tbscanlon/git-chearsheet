# Git Cheatsheet
A quick and dirty guide for using Git via the command line.

## Creating a new Repository
Creating a new repo is very easy. Just navigate to the root folder of your project and run `git init`. This will make a hidden `.git` directory and allow for version control.

### Example
```
cd ~/Projects/cool-new-js-framework/
git init
Initialised empty Git repository in /home/tom/Projects/cool-new-js-framework/.git/
```

You can also use `git clone` to make a local copy of an existing repository.

***Note:*** *When cloning from Github, you'll need the SSH link to the project. This can be found by clicking on the green "Clone or download" button on the project's main page.*

### Example
```
cd ~/Projects
git clone git@github.com:tbscanlon/ruby-toys.git
Cloning into 'ruby-toys'...
remote: Counting objects: 26, done.
remote: Total 26 (delta 0), reused 0 (delta 0), pack-reused 26
Receiving objects: 100% (26/26), done.
Resolving deltas: 100% (6/6), done.
```

## Basic Snapshotting
| Command        | Description           | Example  |
| -------------- |---------------------| --------|
| `git add` | Adds a file to the staging area | `git add main.rb` |
| `git status` | View the status of files in the working directory and staging area | `git status` |
| `git diff` | Shows differences between modified and staged files | `git diff` |
| `git commit` | Records a snapshot of the staging area | `git commit -m "Final commit. Goodbye cruel world."` |
| `git rm` | Removes files from the staging area | `git rm compromising_photos.zip` |

## Branching and Merging
| Command        | Description           | Example  |
| -------------- |---------------------| --------|
| `git branch` | List, create and manage branches | `git branch top-secret` |
| `git merge` | Merge a branch into your current one | `git merge dev` |
| `git log` | Show a branch's history | `git log --oneline --graph` |
| `git checkout` | Move between branches and commits | `git checkout faba307aa` |

## Sharing and Updating
| Command        | Description           | Example  |
| -------------- |---------------------| --------|
| `git remote add` | Add a new remote repository | `git remote add origin git@github.com:tbscanlon/git-cheatsheet.git` |
| `git remote rm` | Removes an exisiting remote alias | `git remote rm origin` |
| `git fetch` | Download new branches and data from a remote repo | `git fetch origin` |
| `git pull` | Fetch from a remote repo and try to merge into the current branch | `git pull origin` |
| `git push` | Push new branches and data to a remote repository | `git push origin master` |

## Inspection and Comparison
| Command        | Description           | Example  |
| -------------- |---------------------| --------|
| `git log` | View and filter commit history | `git log --author=tbscanlon` |
| `git diff` | See absolute changes between two commits | `git diff faba307aa` |
