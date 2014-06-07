GulpJS Development Environment
====================

My version of a GulpJS development environment. It utilizes browserify so you can use `require()` in your client-side javascript. Mocha and should.js are used for unit testing which are run automatically before every gulp restart. LESS is used as the CSS preprocessor and finally it grabs javascript dependencies from `./vendor`. If you use Bower from within this environment they will be placed automatically into `./vendor`.

All javascript is concatenated and uglified prior to being placed into `./public/js/` where you will find two files, `app.js`, and `app.min.js`. CSS is concatenated, minified and placed into `./public/css/screen.css`.

## Quickstart
	
	gulp

## Options
	
	NODE_ENV=dev gulp

Starts the environment and invokes the watch command which will automatically scan for changes in `./lib/*.js`, `./less/*.less`, `./test/*.js`, and `*.html` files.

## License

[MIT](https://github.com/isfinite/gulp-dev-env/blob/master/LICENSE)