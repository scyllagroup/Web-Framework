<div class="breadcrumbs">
[Documentation](/) / Foundation / Getting Started / Setup and Configuration
</div>

# Setup and Configuration

## Starting a New Project

New projects can be started by any team member. Visit our [Git repository](http://git.scylla.local/Repository/Index) to create new projects. Under the **Scylla** header you'll find a project called **webframework-ui**. Click this project to view the detail page. You can then use the clone button to create your new project from the latest and greatest version of the web framework.

Convention is important and will help us maintain a clean and organized repository. Please use the website address followed by a hyphen (-) and finally the word design. For example: **scyllagroup.com-design**, or use the client name **scyllagroup-design**.

```
git clone http://git.scylla.local/WebFramework.git
```
One of the first things you want to do with a new framework project is ensure all the node packages are installed correctly. This can be accomplished in two different ways. The first is to just run `npm install`. The second, and recommended way, is to run `npm install -g yarn` to globally install the **yarn** package. This is a more efficient way of getting all the necessary node components installed properly. After it's been installed, just run the command `yarn` and all your node packages will be downloaded. The easiest way to make sure you're scoped to your project when you run these commands is to use the integrated terminal within Visual Studio Code. This will open a terminal right in your window, within the correct working directory.


### Installing a Project Locally

<!-- ### Required Software

1.  Install [Git](https://git-scm.com/downloads)
    *   When asked if you would like Git to run from its own command window, select the 2nd option to run it from the windows command line too.
    *   When asked about line endings, select the 3rd and last option so that Git does not force or change line endings at all.
2.  Install [NodeJS](https://nodejs.org/en/download/)
3.  Install [Visual Studio Code](https://code.visualstudio.com/#alt-downloads) -->

If you have any trouble at all please refer to the "readme.md" file. It is located at the root directory of your project and you should be able to open and read it with Visual Studio Code. It should contain the latest instructions on how to build and run the project.

1.  Visit our [Git repository](http://git.scylla.local/) and find the project you want to work on.
2.  Copy the **General Url** for the project.
3.  Open up the **command prompt** or **terminal**.
4.  Use the "cd" command to change the current directory to your working directory. Most likely **cd c:/git/**.
5.  Use Git to clone the project by running the following command: **git clone {{General Url}}**. To paste the Url in place (without curly braces) you may need to use the right mouse button.
6.  Type in your password if you are asked for it. This is the same as your Windows login.
7.  If successfull, you should see a brand new folder in your working directory. Most likely **c:/git/name-of-project/**.
8.  Use the "cd" command again to switch into your new project directory. Then run ``npm install``, or ``yarn``.
9.  To run the project in your browser use `npm run serve`, or for older projects, run `gulp serve`.

### The Git Repository

Working with Git enables us to save our changes at major milestones, share code and collaborate on a project as a team, and have a working history of changes in case we need to rollback some updates.

It's good practice to always **pull down the latest changes** for a project everytime you go to work on it.

All of your work is performed locally on your machine. As you make changes to files they are recorded locally, and you can **commit changes** at anytime. After fully testing & validating your changes on your local machine, you can share them with the rest of the team by **pushing or syncing your changes** back to the repository.

There are rare occasions when conflicts may occur and you will not be able to check in your files. When this happens it usually means somebody else has pushed code to the repository that you do not have yet. To continue with your changes, you'll need to **pull** down the latest changes. You may also have to merge conflicts. It's sometimes best to talk to the person who pushed last to verify you are not overwriting any of their work.

#### Working with Local Branches

Branching is important because it allows you to edit code and make changes in an environment that won't affect the remote code base. It will also help you keep track of all your changes within a given project. All projects typically have a master (or release) branch where all the stable code lives. This is where you'll want to base all of your branches off of. Once you copy a project, you'll already be on the master branch. You can create a new branch by typing `git branch {{branchName}}`, and then switch to that branch by typing `git checkout {{branchName}}`. The shorthand way to do this is by typing `git checkout -b {{branchName}}`, which will create a new branch and then check it out for you.

Branch names can have no spaces, and are typically camel cased. Our general rule for branches to is to associate them with a jira ticket. If the ticket name is **TSG-117**, then your branch name should be **jira/tsg-117**, or something similar. This lets you check your branches against your jira tickets, and keep track of what features or code changes that the branch holds.

One of the most important things to remember when working with local branches is to commit your changes when you're done working on that branch for any reason. Commiting changes is how git keeps a record of things you have changed on your branch. Save all your work, then run `git add .` to stage all your files for a commit. Next, run `git commit -m "{{write a commit message here}}, and your changes will be commited, along with the message you wrote.

Once a branch is no longer needed, you should clean up your local git repository by deleting that local branch. You'll need to switch to another branch then run `git branch -D {{branchName}}` to delete the branch.


#### Working with Remote Branches

Remote branches are branches that are saved or **pushed** back to the repository. They exist on a server and are accessible to everyone as opposed to just a local user. The master and development branches for a given project are almost always remote branches, so that everyone on the project can work with them. The only time it is necessary to push a local branch to the repository is if it requires collaboration between multiple project members. If you checkout a remote branch on your machine, you'll create a local instance of that branch. This branch however is tracked by the remote branch. This means that if a change occurs on the remote you can run `git pull` and your version of the branch will be updated to the most recent code push. If you want to add your changes to the remote branch, use `git push` and any commited changes will be pushed to the remote branch for anyone with access to the repo to see.

If you try to push your changes while there are changes on the remote branch that you haven't pulled, git will stop you and tell you to pull changes down before pushing new changes up. 

Typically in a project there are two important remote branches to keep track of. One of these is the **development** branch, and the other is the **master** branch. When building new features, or adding bug fixes, the general process is to pull down the development branch, and then use `git merge` to merge in your local changes. Once that's finished and any merge conflicts are resolved, that branch can be pushed back up to the repo and the new code can be tested in the development environment. Once it's been tested and approved, you can merge the local branch into the master branch so that it can be pushed to the live site. **Never merge development directly into master**! Development should always be the testing envrionment and can contain ustested or unstable code.

#### Creating a Release

TBD.