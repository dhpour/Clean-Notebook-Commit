# Clean Notebook Commit

Ban your nnotebooks commits if their output cells are not empty.

### Usage
Copy `pre-commit` to your repo hooks: 

    cat pre-commit >> .git/hooks/pre-commit
It doesn't change your notebook. ~~It doesn't even `git reset` for you.~~ It unstages files, rejects the commit and remindes you of your notebook cell outputs state for committing if you have forgotten to clean them.

### Dependency
You need [underscore-cli](https://github.com/ddopson/underscore-cli) for using this hook.

    npm install -g underscore-cli
    underscore help

### Similar works
For having more control over the process or manipulating the notebooks you can use [nbstripout](https://github.com/kynan/nbstripout) and [nb-clean](https://github.com/srstevenson/nb-clean).