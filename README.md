# servicedev2
redesign for service.uark.edu

## Features
- CSS Autoprefixing
- Built-in preview server with BrowserSync
-  compile Sass with libsass
- lint scripts automatically
- Map compiled CSS to source stylesheets with source maps
- image optimization
- wire-up dependencies installed with Bower automatically with wiredep
- The gulpfile makes use of ES2015 features by using Babel
- build and deploy to Amazon S3
- revision for css and js files

## Included Frameworks
- bower
- gulp
- bootstrap 4
- fontawesome

## Getting Started
- Install dependencies: npm install --global yo gulp-cli bower
- Install the generator: npm install --global generator-webapp
- Run yo webapp to scaffold your webapp
- Run gulp serve to preview and watch for changes
- Run bower install --save <package> to install frontend dependencies
- Run gulp serve:test to run the tests in the browser
- Run gulp to build your webapp for production
- Run gulp serve:dist to preview the production build

## Bower components
Bower components are moved to root because '/app' is reserved for dev files and not third-party libraries.

### Basically:
* paths in Sass `@import` directives should begin with `bower_components`
* paths in HTML should begin with `/bower_components`

Both paths will work regardless of the nesting level, e.g. they would work on a `about/contact/index.html` page too.

## TODO
- encapsulate components
- comment out each div for departmental reuse
- add FAQ and Documentation
