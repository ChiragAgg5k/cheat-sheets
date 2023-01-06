# Git CheatSheet

created: 2022-11-16 13:26

"_It is easy to shoot your foot off with git, but also easy to revert to a previous foot and merge it with your current leg._" **—Jack William Bell**

This CheatSheet contains all the necessary git commands I use on a daily or semi daily basis. I know there are multiple cheat sheets present on the internet for git (_one of them present in pdfs folder_) but it's always a good idea to make your own versions. Feel free to use this cheat sheet as a reference.

## Basic Commands

These are the basic commands every programmer should learn by heart.

### Initializing a repository

```
cd {path_to_directory}
git init
```

### Cloning a repository

```
cd {path_to_directory}
git clone {url}
```

### Git Status

Shows all the modifications/changes made in the local repository which are yet to be committed.

```
git status
```

### Staging commits

This is a intermediate step before committing to a particular change. It allows you to commit only specific changes, or given the changes different commits with different messages. You can stage all changes at once using **"."** .

```
git add {file_name}
git add . 
```

### Committing changes

This is the main step that finalizes the changes you made. Its literally committing to your file changes. You can skip the staging step by using **"-a"** to directly commit all the modifications.

```
git commit -a
git commit -m "message"
```

### Git Show

Shows the changes committed in detail before pushing them to the local repo. Its output is similar to git log. The difference is by default git show shows details of most recent commit (HEAD). Git log on its own will show all commits made.

```
git show
git show {hash_of_commit}
```

### Git Remote

We need to connect our local repo to remote for the world to see. You can view and add remotes to your local repository using these commands. Note that we typically name the remote "origin" because as the name suggests, it refers to the original remote repo.

```
git remote add {name} "url"
git remote -v
git remote rm {name}
```

Here the "url" is the SSH key your remote repo manager will provide (which in 99.99999% cases is **Github**)

### Git Branch

We also need to select a branch to where we want to push our changes. When creating a file for the first time we need to create a new branch.

```
git branch [new_branch_name]
```

But this alone doesn't automatically make us use the newly created branch. To use the branch use the **checkout** command.

```
git checkout [new_branch_name]
git checkout [new_branch_name] [existing_branch]
```

To list branches:

```
git branch
```

To delete a branch:

```
git branch -d [branch_name]
```

Oof that was a lot. Branches are super useful but can be hard to organize. Thats why i would highly recommend using git branch visualizers, there are a lot of them!

### Git Push

Now that we have selected our remote repo, and a branch, we can finally push are committed changes.

```
git push -u {remote name} {branch name}
```

Now here **"-u"** is used to set upstream on the branch. What is upstream you ask? GOOD QUESTION. Its basically important if you want someone to pull your repo, otherwise it gives error or something. Just use it, don't ask questions.

## Non Basic Commands

The rest of these commands need not be learned by heart, but once you become experienced enough, you will learn them automatically.

### Git Log

This command's life has been taken by many git history visualizers. Still the OGs rely on it. It shows a list of past commits along with their commit ids, which can then be used to show each commit in detail.

```
git log
```

``` 
git log --oneline --graph
```

### Git Diff

This command shows the difference between the current state of the file and the last commit. It can be used to see the changes made in the file before committing them.

```
git diff
```

### Git Reset

This command is used to revert to a previous commit. It can be used to revert to a previous commit, or to unstage a staged commit. It can also be used to revert to a previous commit and stage it.

```
git reset {commit_id}
git reset HEAD
git reset --soft {commit_id}
```

### Git Revert

This command is used to revert to a previous commit.

```
git revert {commit_id}
```

### Git Merge

This command is used to merge two branches. There can be two types of merges, fast-forward and three-way. Fast-forward is when the branch you are merging into is ahead of the branch you are merging. Three-way is when the branch you are merging into is behind the branch you are merging. The three-way merge is the default merge.

```
git merge {branch_name}
```

### Git Pull

This command is used to pull changes from a remote repository. It is basically a combination of git fetch and git merge.

```
git pull
```




