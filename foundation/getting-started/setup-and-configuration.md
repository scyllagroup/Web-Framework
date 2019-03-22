<div class="breadcrumbs">
[Documentation](/) / Foundation / Getting Started / Setup and Configuration
</div>

# Setup and Configuration

## Install the Necessary Dependencies

You'll first need to install the following software on your computer. 

<p class="warning">If you have Visual Studio installed, you may also have NodeJS installed already.</p>

* [NodeJS (v8.10.0)](https://nodejs.org/dist/v8.10.0/)
* [Git](https://git-scm.com/downloads)
* [Visual Studio Code]() (Optional)
* Yarn (Optional)

Install yarn by running the following command in the *command line* or *terminal*:

```
npm i yarn -g
```

## Download & Install the Web Framework

In your *command line* or *terminal* you can now use the `git` command to pull down the Web Framework. You'll then install the dependencies using the package manager bundled with NodeJS `npm`, or you can use `yarn` (another optional install but our recommended package manager).

<p class="warning">If you don't want to use *yarn* simply replace `yarn` with `npm i` in the commands below.</p>

```
git clone https://github.scyllagroup.com/Scylla/web-framework
cd web-framework
yarn
```

## Install the SSL Certificate for Local Development

<p class="danger">These instructions are for Windows users. Mac users will need to research how to import and trust our self-signed certificate <em>my-cert.pfx</em>.</p>

To avoid the "invalid certificate" error from your browser when running the Web Framework we've created a self-signed SSL certificate. You'll need to import this file using the `importcert.ps1` script at the root folder. This script will import the `my-cert.pfx` file, and then browsers should recognize and trust the certificate moving forward.

### Using the Web Framework

Now that you have the necessary software isntalled and you've cloned the project to your computer you can begin using the Web Framework. The Web Framework uses a package called BrowserSync that spins up a local web server so you can view your work in real-time, synced across multiple browsers if you choose to. The command to start the server is simply: 

```
npm run serve
```

If you open up the `package.json` file you will find other commands are available.

## Starting a New Project

More often than not the reason we need to download and install the Web Framework is to create a new UI/UX prototype for a new project. The steps are the same as above under **Download & Install the Web Framework** but afterwards you will need to:

1. Delete the `/git` folder.
2. Run `git init` from the *command line* or *terminal*
3. Create a version branch `git checkout -b release/1.0.0`
4. Make your first commit `git commit -m "web framework init"`

You are now ready to create a repo and upload this branch. Create a new project in [GitHub Enterprise](https://github.scyllagroup.com/). Try to follow a naming convention such as `client-ui` or `domain.com-ui`.

After creation you'll be given instructions on how to **...or push an existing repository from the command line**. It's similar to this, but make sure you use the commands they provide to you:

```
git remote add origin https://github.scyllagroup.com/client/project.git
git push -u origin release/1.0.0
```  

You've successfully cloned the Web Framework and started a new repo in GitHub Enterprise.