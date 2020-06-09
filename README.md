## The_Girl_Code_Blog

> This blog was developed as part of a project by #Build Program of Girlscript Foundation .
> It was made using HTML,CSS and Bootstrap and more functionalities will be added soon in the blog .

## Steps to follow :

### 1. Fork it :

You can get your own fork/copy of [internship](https://github.com/coderplex/internship) by using the <a href="https://github.com/coderplex/internship"><kbd><b>Fork</b></kbd></a> button .

[![Fork Button](https://help.github.com/assets/images/help/repository/fork_button.jpg)](https://github.com/coderplex/internship)

### 2. Clone it :

You need to clone (download) it to local machine using

```
$ git clone https://github.com/Your_Username/internship.git 
```

> This makes a local copy of repository in your machine.

Once you have cloned the `internship` repository in Github, move to that folder first using change directory command.

```sh
# This will change directory to a folder internship
$ cd internship
```

Move to this folder for all other commands.

### 3. Set it up :

Run the following commands to see that *your local copy* has a reference to *your forked remote repository* in Github :

```sh
$ git remote -v
origin  https://github.com/Your_Username/internship.git (fetch)
origin  https://github.com/Your_Username/internship.git (push)
```

Now, lets add a reference to the original [internship](https://github.com/coderplex/internship) repository using

```sh
$ git remote add upstream https://github.com/coderplex/internship.git
```

> This adds a new remote named ***upstream***.

See the changes using

```sh
$ git remote -v
origin    https://github.com/Your_Username/internship.git (fetch)
origin    https://github.com/Your_Username/internship.git (push)
upstream  https://github.com/coderplex/internship.git (fetch)
upstream  https://github.com/coderplex/internship.git (push)
```

### 4. Sync it :

Always keep your local copy of repository updated with the original repository.
Before making any changes and/or in an appropriate interval, run the following commands *carefully* to update your local repository.

```sh
# Fetch all remote repositories and delete any deleted remote branches
$ git fetch --all --prune

# Switch to `master` branch
$ git checkout master

# Reset local `master` branch to match `upstream` repository's `master` branch
$ git reset --hard upstream/master

# Push changes to your forked `internship` repo
$ git push origin master
```

Once you have completed these steps, you are ready to start contributing by checking our `Help Wanted` Issues and creating [pull requests](https://github.com/coderplex/internship/pulls) .

### 5. Create a new branch :

Whenever you are going to make contribution. Please create seperate branch using command and keep your `master` branch clean (i.e. synced with remote branch).

```sh
# It will create a new branch with name Branch_Name and switch to branch Folder_Name
$ git checkout -b Folder_Name
```

Create a seperate branch for contibution and try to use same name of branch as of folder.

To switch to a desired branch

```sh
# To switch from one folder to other
$ git checkout Folder_Name
```

To add the changes to the branch, use

```sh
# To add all files to branch Folder_Name
$ git add .
```

Type in a message relevant for the code reveiwer using

```sh
# This message gets associated with all files you have changed
$ git commit -m 'relevant message'
```

Now, Push your awesome work to your remote repository using

```sh
# To push your work to your remote repository
$ git push -u origin Folder_Name
```

Finally, go to your repository in browser and click on `compare and pull requests`.
Then add a title and description to your pull request that explains your efforts.

## >To contribute to the [Learnplex Project](https://github.com/coderplex/learnplex) , please refer to the Prerequisites and Installation section of [Learnplex Docs](https://docs.coderplex.in/) . 