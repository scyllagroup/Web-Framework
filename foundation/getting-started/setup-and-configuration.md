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

### Installing a Project Locally

<!-- ### Required Software

1.  Install [Git](https://git-scm.com/downloads)
    *   When asked if you would like Git to run from its own command window, select the 2nd option to run it from the windows command line too.
    *   When asked about line endings, select the 3rd and last option so that Git does not force or change line endings at all.
2.  Install [NodeJS](https://nodejs.org/en/download/)
3.  Install [Visual Studio Code](https://code.visualstudio.com/#alt-downloads) -->

If you have any trouble at all please refer to the "readme.md" file. It is located at the root directory of your project and you should be able to open and read it with Visual Studio Code. It should contain the latest instructions on how to build and run the project.

1.  Visit our [Git repository](http://git.scylla.local/) and find the project you want to work on.
2.  Copy the **personal URL** for the project.
3.  Open up the **command prompt** or **terminal**.
4.  Use the "cd" command to change the current directory to your working directory. Most likely **cd c:\projects\**.
5.  Use Git to clone the project by running the following command: **git remote add origin {{personal URL}}**. To paste the personal URL in place (without curly braces) you may need to use the right mouse button.
6.  Type in your password if you are asked for it. This is the same as your Windows login.
7.  If successfull, you should see a brand new folder in your working directory. Most likely **c:\projects\name-of-project\**.
8.  Use the "cd" command again to access your new project directory. Then run **npm install**.
9.  To run the project in your browser use **gulp serve**.

### The Git Repository

Working with Git enables us to save our changes at major milestones, share code and collaborate on a project as a team, and have a working history of changes in case we need to rollback some updates.

It's good practice to always **pull down the latest changes** for a project everytime you go to work on it.

All of your work is performed locally on your machine. As you make changes to files they are recorded locally, and you can **commit changes** at anytime. After fully testing & validating your changes on your local machine, you can share them with the rest of the team by **pushing or syncing your changes** back to the repository.

There are rare occasions when conflicts may occur and you will not be able to check in your files. When this happens it usually means somebody else has pushed code to the repository that you do not have yet. To continue with your changes, you'll need to **pull** down the latest changes. You may also have to merge conflicts. It's sometimes best to talk to the person who pushed last to verify you are not overwriting any of their work.

#### Working with Local Branches

TBD.

#### Working with Remote Branches

TBD.

#### Creating a Release

TBD.