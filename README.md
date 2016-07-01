# New project boilerplate 

### Updated newproject:
Updates to the original and some new versions as well. See below for full feature list



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


# V2

All new and improved for unit testing. I have made 3 new versions and improvements on the original. 

### newproject
`newproject` got a simple facelift. It now poplautes the index.html with some basic boilerplate/file paths. Fixed some formatting, and added 'NO' condition.

### newprojectSansGit
does everything `newproject` does except without git. A couple of you mentioned you would prefer to control your git setup yourself. Done and done.

### newprojectJas / jas

```note: wget is required for all jasmine enabled bash scripts```

the exciting stuff. `newprojectJas` takes the base `newproject`, and supercharges it with a Jasmine install. `jas` will initiate Jasmine in an existing project.

1. uses wget to retreive Jasmine
2. unzips into local dir
3. removes superfluous files folders **
4. creates spec file in js dir called testSpec.js
5. automatically sets up SpecRunner.html with appropriate file paths to testSpec.js and main.js
6. adds new lines to .gitignore in order to ignore SpecRunner.js and lib/ as well as adds an optional line (just remove the //) to ignore all spec files.


### * These all install and run the exact same way as `newproject`. Just follow the instrcutions above (but change the file names of course). The file name becomes the command to run * 



**
```A quick note about my choice here. I remove almost everything except the jasmine lib itself, and start over. Create my own SpecRunner.html, and spec.js file (which I place into js/ dir) instead of using `src` and `spec`. This is a personal choice, I happen to think it looks, and feels cleaner. However, I want this to help people, so if it's confusing or you just don't like it, let me know and I will change it back to the default Jasmine install. ```
