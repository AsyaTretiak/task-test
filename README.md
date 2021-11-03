# task-test
Intallation

•  download and install node.js https://nodejs.org/uk/
• open this repository https://github.com/AsyaTretiak/task-test.git
• open folder in code editor
• create a new terminal
 • run the “npm” i command
 • run the “npm run” prepare command
 • run the project with the “gulp” command
 • the final build of the project is started by the “gulp build” command

What's in the settings?

Automated tasks
• minification of css, js, html
• Image optimization
• browser auto-refresh
• preparation of  styles
• loading js dependencies via npm
• uploading files to the server via ssh
• validation of html on w3c
• archiving dist files and app folders
• tracking file changes
• generation of style files and templates


File structure 

• app - project source files
• dist - the result of gulp build
• node modules - installation files for node.js plugins
• editorconfige- file with settings for the editor.
• Gitignore - folder with installation files, which does not go to Git
• stylelintrc -checks the semantics of the code
• gulpfile.js - folder containing gulpfile and tasks.
• package.json - package settings
• package-lock.json - local package settings

App folder content

• css - general project styles file
• fonts - connected fonts
• images - project pictures,
• js - scripts
• sass - the blocks from which the pages will be built.

How does it work?

Gulpfile.js describes tasks that perform certain actions. All gulp plugins are loaded automatically from package.json using the gulp-load-plugins plugin.
This reduces the size of the gulpfile. In the process, Gulp takes a file from 1 folder, performs the necessary operations with it and saves it to another folder.

NPM and Gulp run commands

• npm i - install npm
• npm run production - run gulp production
• gulp - run gulp
• gulp-build - start project build

Gulp

• styles - sass compilation
• styles: min - csso minification
• styles: rtl - variant of styles from right to left
• scripts: min - js minification
• images - transfer images from src to dist
• images: min - optimization of images in dist
• templates - compilation of jade templates
• sprites - assembly of sprites
• watch - tracking file changes
• browsersync - browser auto-update
• archive - archiving dist and src folders
• archive: dist - archive dist
• w3c: html - html code validation
