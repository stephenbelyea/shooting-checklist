# GruntJS Boilerplate v2.3 #


Basic Grunt setup for Faren projects. This is an ongoing repo, so changes are bound to happen.

**NOTE**: The project is currently running jQuery v1.11.1 (2014-10-07) for old IE support. To update the jQuery library, delete `jquery-1.11.1.min.js` from the `js/libs` directory and dump in a new version. This will automatically concat into `production.min.js` when the `$ grunt watch` handler fires.



## Getting Started ##

1. You will need `Node.js`, `npm`, and `grunt-cli` up and running on your machine. _Take a look at [Grunt's documentation](http://gruntjs.com/getting-started) to get caught up_.

2. Clone this baby into your new project directory.

3. Update the `package.json` file with the project name and description.

4. Via command line, `$ cd` into the project's root directory.

5. Run `$ npm install` and Grunt will setup all dependencies specified in the `package.json` file. _Use_ `$ sudo` _if the install rejects_.

6. Once everything is installed, the `Gruntfile.js` should be configured to allow you to run the `$ grunt watch` command (again, from the root directory) and all necessary sub-directories will be generated.

7. (Bonus for Git) If you're tracking the new repo via Git, pull the `.txt` off of the `gitignore.txt` file and prefix a `.` on the filename. You should wind up with `.gitignore`. Use this to drop tracking of extraneous task files / directories that will be overwritten anytime `$ npm install` is run on a new machine anyway.



## Version Notes ##

### Version 2.3 ###
* Add meta tags for description and author.
* New home under personal GitHub. 

### Version 2.2 ###
* Add markup, message and styling for `<noscript>` fallback.
* Add markup, message and styling for IE < 9 with update link.

### Version 2.1.1 ###
* Fix starting version number in `package.json`. Must be minimum 1.0.0 for install to fire.
* Add transition timing to button background / colour change on hover.
* Add `gitignore.txt` template file.

### Version 2.1 ###
* Core SASS Mixins added for media queries (iPhone P/L, iPad P/L, laptop, desktop) and retina (1.75x) resolution, along with prefixed CSS Animation and Keyframes.
* Basic CSS styling attached to `.default` body class and simple cleanup of CSS Reset at start of `global.scss` file.
* Basic JS `$win` object setup to collect window width, height, and scroll position with JS listeners for window resize and document scroll setup to repopulate.
* NOTE: _Changes are untested with Grunt deployment. Some fixes may be required after testing_.

### Version 2.0 ###
* Changes made based on [Chris Coyier's Grunt Boilerplate](https://github.com/chriscoyier/My-Grunt-Boilerplate).
* Tasks broken out as individual files and grouped in `tasks` subdirectory. Gruntfile setup to allow new tasks by adding file to subdirectory. 
* JS Hinting added to task stack.
* CSS minification broken out as separate task, after SASS preprocessing and prefixes.
* Imagemin added to automated tasks. 

### Version 1.0 ###
* Initial version, includes basic setup.
* Set to run JS concat / minification, SASS processing, CSS prefixing and minification on `$ grunt watch` automation.
* Set to run image compression on manual `$ grunt` fire.
