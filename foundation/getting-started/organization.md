<div class="breadcrumbs">
[Documentation](/) / Foundation / Getting Started / Organization
</div>

# Organization

## Where to Find Things

The Web Framework has a specific file and folder structure. The table below summarizes what each folder holds and references specific files you should be familiar with. 

<p class="tip">
For more information about how the front-end code works please read the [Guidelines for CSS](GuidelinesForCSS) and [Guidelines for JS](GuidelinesForJS).
</p>

<p class="danger">
Some files are hidden from view in Visual Studio Code. These files are rarely edited – hiding them reduces some of the clutter in the tree view, and makes the project much easier to navigate. If for any reason you may need to edit a hidden file, you can toggle it's display value in the workspace settings file. You can also use the search feature to find a specific file.
</p>

### Contributing to the Web Framework

|Folder or File|Details|
|--------------|-------|
|**/.vscode/**|This folder contains workspace settings specific to Visual Studio Code and allows everyone to use the same settings across computers and environments.|
|**/dist/**|**Do not make changes** to files and folders in this location. The `npm run serve` command will build and minify your files from both `framework` and `src` folders, and then serve a web site from this folder.|
|**/framework/**|If you are contributing to the Web Framework, your work will consist of editing files in this directory. Otherwise, you should not edit anything in this directory.|
|/framework/.api/||
|/framework/.build/||
|/framework/.tests/||
|/framework/components/||
|/framework/elements/||
|/framework/layout/||
|/framework/mockup/||
|/framework/pwa/||
|/framework/utilities/||
|**/src/**|**Do not make changes** to files and folders in this location.|
|/src/media/|The 1 exception to the rule, as media assets (images, fonts, etc) need to be placed in this folder.|

### Contributing to a UI Project

|Folder or File|Details|
|--------------|-------|
|**/.vscode/**|This folder contains workspace settings specific to Visual Studio Code and allows everyone to use the same settings across computers and environments.|
|**/dist/**|**Do not make changes** to files and folders in this location. The `npm run serve` command will build and minify your files from both `framework` and `src` folders, and then serve a web site from this folder.|
|**/framework/**|**Do not make changes** to files and folders in this location.|
|**/src/**|Your working folder. You'll find a number of folders created here, and you can create whatever folder structure best fits the project. There are some specific folders we will mention below.|
|/src/media/|Stores all the media assets for the project, and media will be optimized and copied to the `dist` folder on build.|
|/src/||
