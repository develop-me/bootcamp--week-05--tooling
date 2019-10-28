# Methods to see what's happening

1) **Common sense check**

    Use `git status` as a quick way to see what is going on in your project

1) **Recent history**

    Use `git log` to see the recent changes in your project.
    \
    
    If your history is too long for your terminal window you'll end up with a `:` prompt at the bottom, as you can use your cursor to go up and down the log. Use `q` to quit.

1) **Rcnt hstry**
    
    Use `git reflog` to see the recent changes in your project, in a shorter format.
    \
    
    Study the information and try to relate to the changes you've made and commands you've run.
    \
    
    *`history` is a good command to know to show recent things you've run*

1) **See differences**

    Make a change to a file, save it and use `git diff` to see how you can use the `diff` tool to see what has changed.
    \
    
    Useful if a `git status` shows things have been modified but you're not sure what or can't remember what you changed.
