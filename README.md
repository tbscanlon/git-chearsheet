# Git Cheatsheet
A quick and dirty guide for using Git via the command line.

## Creating a new Repository
Creating a new repo is very easy. Just navigate to the root folder of your project and run `git init`. This will make a hidden `.git` directory and allow for version control.

### Example
```cd ~/Projects/cool-new-js-framework/
git init
Initialised empty Git repository in /home/tom/Projects/cool-new-js-framework/.git/
```

You can also use `git clone` to make a local copy of an existing repository.

***Note:*** *When cloning from Github, you'll need the SSH link to the project. This can be found by clicking on the green "Clone or download" button on the project's main page.*

### Example
```cd ~/Projects
git clone git@github.com:tbscanlon/ruby-toys.git
Cloning into 'ruby-toys'...
remote: Counting objects: 26, done.
remote: Total 26 (delta 0), reused 0 (delta 0), pack-reused 26
Receiving objects: 100% (26/26), done.
Resolving deltas: 100% (6/6), done.```
