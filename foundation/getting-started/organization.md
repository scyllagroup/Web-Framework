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
|**/dist/**|**Do not make changes** to files and folders in this location. The `npm run serve` command will build and minify your files from both `/framework/` and `/src/` folders, and then serve a web site from this folder.|
|**/framework/**|If you are contributing to the Web Framework, your work will consist of editing files in this directory. Otherwise, you should not edit anything in this directory.|
|/framework/.api/|This folder contains special routes to allow for prototyping API calls. Each folder (or JSON file) is treated as an endpoint and served back when you make a request.|
|/framework/.build/|Contains scripts needed for building the project.|
|/framework/.tests/|*Not implemented yet.* Mocha and BrowserSync tests specifically for core elements, components, and utilities from the Web Framework and mockup site.|
|/framework/components/|HTML, CSS, and JS for *components*.|
|/framework/elements/|HTML and CSS for *elements*.|
|/framework/layout/|HTML and CSS for *page layout*.|
|/framework/mockup/|A fully working mockup site that showcases our components, elements, and utilities in action.|
|/framework/pwa/|*Not implemented yet.* Example Progressive Wab App.|
|/framework/utilities/|JS code that provides static functions, extensions, and helpers. Typically *shared code between components*.|
|**/src/**|**Do not make changes** to files and folders in this location. (*)|
|/src/media/|(*) The 1 exception to the rule. Store all the media assets for the project, and media will be optimized and copied to the `/dist/` folder on build.|

### Contributing to a UI Project

|Folder or File|Details|
|--------------|-------|
|**/.vscode/**|This folder contains workspace settings specific to Visual Studio Code and allows everyone to use the same settings across computers and environments.|
|**/dist/**|**Do not make changes** to files and folders in this location. The `npm run serve` command will build and minify your files from both `/framework/` and `/src/` folders, and then serve a web site from this folder.|
|**/framework/**|**Do not make changes** to files and folders in this location.|
|**/src/**|Your working folder. You'll find a number of folders created here, and you can create whatever folder structure best fits the project. There are some specific folders we will mention below.|
|/src/media/|Store all the media assets for the project, and media will be optimized and copied to the `/dist/` folder on build.|
|/src/media/fonts/|*Not implemented yet.* Special folder for font files.|
|/src/media/sprits/|*Not implemented yet.* Special folder for SVG files, which will be built into a spritesheet.|
|/src/media/themes/|Contains SVG files specifically for the integration with Umbraco CMS.|
