### Change the remote branch that your Git repository is pointing to

#### ***List Your Remote Branches***

```bash
git ls-remote --heads <remote-name>
```
Replace `<remote-name>` with the name of your remote, typically `origin`

#### ***Update Your Local Branch***

To change the remote branch that your local branch is tracking, run

```bash
git branch -u <remote-name>/<new-branch-name>
```
Replace `<remote-name>` with the name of your remote, typically `origin` and `<new-branch-name>` with the name of the remote branch you want to track.

For example, if you want to make your local branch "my-branch" track the remote branch "feature-branch" on the "origin" remote, you would run:

```bash
git branch -u origin/feature-branch
```

#### ***Fetch the Changes***

After updating the tracking information, it's a good practice to fetch the latest changes from the remote repository to make sure your local branch is up to date with the new remote branch. You can do this with:

`git fetch`

#### ***Check the Branch Status***

You can verify that your local branch is now tracking the correct remote branch by running:

`git branch -vv`

This command will display a list of your local branches with information about their upstream branches.
