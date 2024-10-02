# Bonus

## Setting up Branches
Assuming you are already on the directory (or folder) of your repo, this is how you set up a new local branch.

{% hint style="info" %}
   Like with commits, new branches are first created locally, then uploaded or pushed to remote later in the process.
{% endhint %}

In the terminal:
```
git checkout -b branchName
```
{% hint style="info" %}
   This creates a new branch with the name that you specified, and _automatically_ sets it to your current branch.
{% endhint %}

To check that you have created a new branch and are currently set to it:
```
git branch -a
```
{% hint style="info" %}
   Notice that there are currently THREE "branches":
   > - \* The Branch You Just Created

   > - main

   > - remotes/origin/main
{% endhint %}

- The `*` denotes the branch you are currently on. In this case, since we used `git checkout -b BranchName` earlier, it created and set us up on that branch.

- Branches written in `red` text means that they are `remote` branches which currently exist in the `remote` repository. We'll come back to that later.

## Working on a new branch...

All git operations are basically the same even when you are working on a `branch`. The `git` commands that we've learned (`add`, `status`, `commit`, and `push`) will all still work as intended.

Try making changes to your any of your files, and proceed to `add`, and then `commit` those changes. **BUT DON'T PUSH IT JUST YET**.

But before we start pushing our code, we have to make sure that the `branch` that we made also exists in the `remote` repo!

{% hint style="info" %}
   Do a `git branch -a` again just to see all the `local` and `remote` branches you have set up!
{% endhint %}

Our local branch has to match with a remote branch before we can push, and in order to do that, we do the following command:

```
git push --set-upstream origin BranchName
```

This command enables the first time you `push`. All other `pushes` after this can just be done with `git push` (no need to include all the other commands!).

## Pull Requests!!!

It doesn't end at doing `push` into your new branch. Remember that `branches` exist for the purpose of being merged back into `main`, and mostly acts as a `staging` are for any new features or changes that you want to implement. This is especially helpful when working in teams, so you know exactly who was working on what, and makes `merge`s easier!

Pull Requests are basically merges that you are forced to do in order to pull back `branches` into `main`. You could do this in the terminal, or just on the GitHub website, and I suggest that you do it on the website instead since it's easier to see and approve any changes!

**no screenshots here because no time but just ask me!**