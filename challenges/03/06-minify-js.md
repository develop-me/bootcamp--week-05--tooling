# Combine then minify JS files

Gulp functions you'll need:

- `src()` - find source files
- `concat()` - from gulp-concat package to combine files
- `uglify()` - from gulp-uglify-es package to minify
- `dest()` - save file(s) to destination

## Useful `src()` tips

`src()`'s argument is a file path, or array of filepaths, for example:

`src('js/*.js')`

`src(['js/script1.js', 'js/script2.js'])` - *Note the use of an array `[]` here*

You can also exclude certain files with `!`:

`src(['js/*.js', '!js/not-this-script.js'])`