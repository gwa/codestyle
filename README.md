jscodestyle
===========

## JS

`rc` files for:

- jshint
- jscs

## Grunt tasks

~~~~~~~~.js
// package.json
"devDependencies": {
	"grunt": "^0.4.4",
	"grunt-contrib-jshint": "^0.10",
	"grunt-jscs": "^0.6"
}
~~~~~~~~

~~~~~~~~.js
// Gruntfile.js
jscs: {
	"options": {
		"config": "bower_components/gwa-codestyle/rc/.jscsrc"
	},
	"src": "src/js/*.js"
},
jshint: {
	"options": {
		"jshintrc": "bower_components/gwa-codestyle/rc/.jshintrc"
	},
	"src": [
		"src/js/*.js"
	]
}
~~~~~~~~

