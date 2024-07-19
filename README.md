# Clean Notebook Commit

Ban your nnotebooks commits if their output cells are not empty.

### Usage
Copy `pre-commit` to your repo hooks: 

    cat pre-commit >> .git/hooks/pre-commit
It doesn't change your notebook. It doesn't even `git reset` for you. It only reject the commit and remindes you of your notebook cell outputs state for committing if you have forgotten to clean them.

### Dependency
You need [underscore-cli](https://github.com/ddopson/underscore-cli) for using this hook.

    npm install -g underscore-cli
    underscore help