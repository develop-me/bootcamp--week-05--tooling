# Combine then minify JS files

You're going to build a website in teams for the rest of the week.

Pick an existing website and copy that. You can always use the [DevelopMe.tech site](https://developme.tech/) if you like.

**Please not design your own site** as we want you to practice your developer skills, not your designer one. 

Steps:

1) [Planning](#step-1-planning)
1) [Getting Set Up](#step-2-getting-set-up)
1) [Setup workflow](#step-3-setup-workflow)
1) [GitHub Pages](#step-4-github-pages)
1) [Best practice](#step-5-best-practice)
1) [Minify HTML](#step-6-minify-html)
1) [Auto-refresh browser](#step-7-auto-refresh-browser)


## Step 1: Planning

Plan your website's purpose in your team.


## Step 2: Getting Set Up

### Do only once (on 1 computer, "pair" programming-style):

1) [Create a new GitHub repository](https://github.com/new) for your project, invite your teammates to it (Settings > Collaborators)

1) Add npm and gulp to your project

1) Install the packages from our previous example

1) Add the appropriate files to GitHub using `git add`, `git commit` etc., **include the `package.json` as your team can use this to install the same dependencies**

### Other people in team can then

1) Checkout the GitHub repository locally, use `git clone {repo URL} {optional folder name}` for this

1) Install dependencies from `package.json` with `npm install`

### Start work

Each person in the team can now make some changes, start using the gulp tasks, and commit and push changes to GitHub



## Step 3: Setup workflow

1) Implement plugins to handle:
	- compiling Sass to CSS, and minifying your CSS
	- JS combining and minification
	- enforce code style for tabs or spaces
1) Set up gulp tasks to use these plugins
1) Building a site, with a defined Git workflow using gulp



## Step 4: GitHub Pages

Did you know you can use GitHub to host your site?!

The feature, called GitHub Pages, can be enabled by going to Settings on the project repository and choosing how you want to publish in the "GitHub Pages" section.

You can publish from the master or gh-pages branch, or can have a docs/ folder where you put your built site files.

You can then access your GitHub Pages hosted project at: `<username>.github.io/<repo-name>`

E.g. [oliward.github.io/rainbow-drops/](https://oliward.github.io/rainbow-drops/) (try clicking on the page)



## Step 5: Best practice

Once you're team is up and running try to demonstrate best practice.

**Repo is tidy**
- No excess files
- Files and folders logically named and arranged

**Project is portable**
- `package.json` and `gulpfile.js` have everything that is needed to start contributing

**Project well documented**
- `README.md` includes setup instructions, detail on gulp tasks and their intended use. The intended audiance is new developers joining the team. What do they need to know. This file is written in Markdown, [see here for a quick reference guide](https://guides.github.com/features/mastering-markdown/#examples)
- Keep a TODO list or use of GitHub issues to track any bugs or things that need to be done

**Process-driven working practice**
- Using Gitflow or other defined branching process
- Defined roles or review process, this should also be in `README.md`, how can others contribute?



## Step 6: Minify HTML

Use a gulp plugin to remove whitespace from our HTML files to make them smaller.

Consider your approach, as we want to keep the original, unminified HTML too.

### Approach 1
/index-dev.html → /index.html

### Approach 2
/src/index.html → /dist/index.html

### Optional - same approach for all assets
/src/js/scripts.js → /dist/js/scripts.min.js



## Step 7: Auto-refresh browser

Look into, and implement, a gulp plugin that will auto-refresh browser when files change.

Suggested plugin: [Browsersync](https://www.browsersync.io/docs/gulp).

**If you get stuck with this [see Oli's sample](https://gist.github.com/oliward/426a6a89bda3d55c614b495431290ba4)**






