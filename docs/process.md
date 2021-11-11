# Understanding our process

## Branches

A *branch* in Git is a copy of the content of a repository that can contain isolated changes from all others.

All help content repositories use a [trunk-based branching strategy](https://www.atlassian.com/continuous-delivery/continuous-integration/trunk-based-development).  The primary branch, or trunk, is **main**.  The `main` branch reflects what is currently deployed and changes to the branch will automatically be deployed.  Your local work should happen in a feature branch, **not** in your copy of `main`.  Use a branch naming format similar to {summary} (a concise overview of your proposed change).

To create a branch for your work, open a terminal window and navigate to the cloned repository. It is important to always start from an updated version of the `main` branch, especially if you make multiple contributions!  Create a new branch with the following commands:

```shell
git checkout main
git pull upstream main
git checkout -b "{summary}"
```

## Make updates

Now that you have your new branch created, you are free to make changes.  Edit your local copy of the markdown files!  When you are happy with the state of the content and all your files are saved, commit and push your changes.  Only commit updates to files you intended to change.  To see all changed files, run the following:

```shell
git status
```

For each of these listed files, they each need to be staged for your commit.  This is done with the following command:

```shell
git add {file1}
git add {file2}
git add ...
```

Commit your changed files and give a helpful commit message:

```shell
git commit -m "Summary of changes"
```

Finally, you need to push your changes to GitHub.  Perform the following to do that:

```shell
git push --set-upstream origin {summary}
```

:::note
The {summary} in the example is the name of the branch.  It should match the same name you used in the `git checkout -b` command before.
:::

## Pull requests

All changes must be reviewed before they are included in primary branches and deployed.  This is done with a [*pull request*](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests). When creating a pull request on a help content repository, you will select your branch in your account containing changes as the source branch, and the `main` branch of the original *smatechnologies* repository as the target branch.  Reviewers will automatically be notified and added.

Automatic checks run when a pull request is submitted.  If one of these fails, you will be asked to fix the issue before continuing further with the request. There can also be conversations that happen as part of a pull request, and typically reviewers will wait to approve and merge changes until all conversations are resolved.

## Deploying changes

Once the changes have been integrated to the `main` branch, a GitHub action will run to build the new content and deploy it to the <https://help.smatechnologies.com> website in the appropriate location.  This will happen in a handful of minutes after the commit appears in history.

## Full example

An end-to-end sample of all commands you might run to work locally on your workstation and submit a change request would look similar to:

```shell
git checkout -b "misspelling-in-release-notes"
vim docs/release-notes.md ## make your edits here, likely in Visual Studio Code or another editor
git status
git add docs/release-notes.md
git commit -m "Fixed misspelling of OpCon in release notes"
git push --set-upstream origin "misspelling-in-release-notes"
```

From here, create your pull request, get it approved, and your changes will be reflected on the site!
