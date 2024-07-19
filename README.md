# Clean Notebook Commit

Ban your nnotebooks commits if their output cells are not empty.

### Usage
Copy `pre-commit` to your repo hooks: 

    cat pre-commit >> .git/hooks/pre-commit

### Dependency
You need [underscore-cli](https://github.com/ddopson/underscore-cli) for using this hook.

    npm install -g underscore-cli
    underscore help