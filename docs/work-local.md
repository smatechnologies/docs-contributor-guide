# Working local

For changes that are too involved to be completed in only your web browser, you can use your workstation as a development environment and work with more robust tools.  Large proposals are less likely to be accepted, so please collaborate early and often before significantly overhauling a section of content.  To set up your workstation, complete the following:

## 1. Install tools

Before beginning, you need to make sure you have **Git** and **Visual Studio Code**.

### Install Git

Navigate to [Git](https://git-scm.com/downloads) and select the appropriate version based on operating system.  Follow the instructions for installation.

If prompted, provide a username and email address.

### Install Visual Studio Code

Navigate to [Visual Studio Code](https://code.visualstudio.com) and select the appropriate operating system version.  Follow the instructions to download and install the application.

### Install Node.js

All content repositories are built by [Docusaurus](https://docusaurus.io).  To build or locally browse Docusaurus content, you will need Node.js.  You can [download Node.js here](https://nodejs.org/en/download/).

After following the instructions for your method of choice, open a command prompt and run:

```shell
node -v
```

You should see the command return a version or versions.

## 2. Clone the repository locally

Now that you have the tools for making changes, you need to copy the content to your workstation.  To begin, fork the content repository:

1. Go to the official repository and click the Fork button in the upper-right hand corner of any page.
2. Select an account or organization that you have write access to.

Once you have a fork of the repository that you can maintain, you now must clone the repository to your workstation.

1. Open a command line and change directories to where you would like to keep the repository locally.
2. Run the following command, replacing {username} and {repository} with the relevant information:

   ```shell
   git clone https://github.com/{username}/{repository}.git
   ```

   :::tip Example
   `git clone https://github.com/smatechnologies/docs-contributor-guide.git`

   Do not use this actual command, you will not be able to push updates.
   :::

3. If prompted for credentials, [create a Personal Access Token (PAT)](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token#creating-a-token) if you do not already have one.  Provide your GitHub username and PAT when prompted.

4. The repository should now be located in a directory sharing a name with the repository in the directory you ran the `git clone` command from.

## 3. Start making changes

Congratulations!  Your account and environment now has the proper setup to begin contributing to the content repositories.

Execute the following command to run the content locally:

```shell
cd 'your-cloned-repository'
npm install
npm run start
```

This should launch a browser and reload changes as files are saved.  

:::note
A handful of change types are not supported.  If an error occurs or your change is not represented, you can `CTRL+C` to end the start command and then re-run it.
:::

All of the documentation content is in the `/docs` directory and are markdown files.  See the [Markdown reference](reference.md) for syntax help.

A full test of your changes happens when you build the content entirely.  This is an automatic check as part of every pull request and is required to pass for your change to be integrated.  To do this locally, run:

```shell
npm run build
```

When you are satisfied with the status of your changes, [**read about our process for next steps**](process.md) to get your changes integrated and published!
