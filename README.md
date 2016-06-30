# New project boilerplate


### A simple bash script for setting up new projects quickly and easily

#### This script does a few things:

1. Checks working directory to make sure it is actually where you want to install
1. Creates index.html .gitignore .jshintrc gulpfile.js files in the main directory
1. Creates two sub-directories, css & js, and creates an initial file in each directory
1. Populates .gitignore, .jshintrc, and gulpfile.js with initial setup code
1. Initializes NPM
1. Installs gulp, jshint, jshint-stylish, gulp-watch, gulp-jshint as dev dependencies
1. Initializes a new git repo
1. Makes an initial commit on master


### The rest is up to you!

#### To run (two methods):

##### First method (the obnoxious way):

1. Simply download the newproject.sh file
1. Create a new empty directory and cd into it
1. Copy newproject.sh into new directory
1. run command `sh newproject`

##### Better way: 

1. Download newproject
2. cd into your download dir
3. run `cp newproject /usr/local/bin`
4. Once you have the file copied over, in your terminal (from anywhere) run `chmod +rx newproject`
5. Now whenever you want to start a new project, just create your empty directory, cd into it and run command `newproject`

```note: You will need root privileges for this. Also this is the usr folder at the root of your computer. NOT the User/ folder.```

Voila! You have a brand new project ready to go!
