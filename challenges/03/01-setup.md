# Prime your repo for use with gulp

1) **Clone project**

    Template site repository on GitHub: [https://github.com/develop-me/gulp-template](https://github.com/develop-me/gulp-template)

    *Remember: `git clone` will make a new folder wherever you are in terminal, so `cd` to the right place or `pwd` to check where you are.*


1) **Initiate npm**

   `npm init --yes`


1) **Install the gulp package**

   `npm install gulp`

   Check `package.json` has auto-updated


1) **Add a .gitignore file to manage the madness that is /node_modules**

	`touch .gitignore` 

	`code .gitignore` and add `/node_modules'

    save your file
	
	use either VSCode or `git status` to see that it's worked

1) **Tour of the site**

    Open `index.html` in the browser and have a review of the site.

    This is a [Bootstrap v4](https://getbootstrap.com/docs/4.3/examples/) site.

    Uses Sass, compiles `scss/styles.scss` to `css/styles.css`, from many Sass files

    Uses some JavaScript files (see bottom of `index.html`):
    - `js/jquery-3.3.1.slim.js`
    - `js/popper.js`
    - `js/bootstrap.js`


1) **Add an emoji to slack to let the instructor know you have finished**	