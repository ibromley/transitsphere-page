### Project Structure

Where is everything located? Here is a brief overview of how our project is laid out.

```
    ├── build - generated, not checked in but deployed to gh-pages branch
    │   ├── assets
    │   ├── app.js
    │   ├── index.html
    │   └── style.css
    ├── data - folder for all JSON data files
    ├── Gruntfile.js
    ├── package.json - Node dependencies and metadata
    ├── project.json - various project configuration
    ├── src
    │   ├── assets - files will be automatically copied to /build
    │   ├── css
    │   │   └── seed.less
    │   ├── index.html
    │   └── js
    │       ├── main.js
    │       └── lib - directory for odd modules
    └── tasks - All Grunt tasks
        ├── lib - directory for Browserify modules
        ├── build.js
        ├── bundle.js
        ├── clean.js
        ├── connect.js
        ├── copyAssets.js
        ├── cron.js
        ├── ghpages.js
        ├── less.js
        ├── loadJSON.js
        ├── loadSheets.js
        ├── state.js
        └── watch.js
```

