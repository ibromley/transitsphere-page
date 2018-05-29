# Grunt Tasks

The default Grunt task built into the template will run all the build
processes, start the dev server, and set up watches for the various
source files. Of course, you can also run these as individual tasks,
including some tasks that do not run as a part of the normal build.
Remember that you can use ``grunt --help`` to list all tasks included in
the project.

## What's Included?

-  `json` - Load JSON files onto ``grunt.data.json``
-  `sheets` - Download data from Google Sheets and save as JSON files
-  `template` - Load data files and process HTML templates
-  `less` - Compile LESS files into CSS
-  `bundle` - Compile JS into the app.js file
-  `connect` - Start the dev server
-  `watch` - Watch various directories and perform partial builds when
   they change
-  `deploy` - Push contents of `build` folder to the `gh-pages` branch for hosting

The deploy task deserves a little more attention. When you run `grunt deploy`, it will rebuild your project in the same way as the default task. The task will then push the contents of the `build` folder up to Github Pages. You will be prompted for your Github credentials if they are not locally cached.