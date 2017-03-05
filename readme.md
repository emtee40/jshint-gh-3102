# Investigation for gh-3102

This repository is intended to isolate a bug in JSHint that was initially
reported in [JSHint issue
gh-3102](https://github.com/jshint/jshint/issues/3102).

## Setup

Run the following command from the root of this project:

    $ npm install

## Testing

The following commands demonstrate the expected behavior of the JSHint
command-line interface:

    $ ./node_modules/.bin/jshint --version
    jshint v2.9.4
    $ ./node_modules/.bin/jshint myscript.js 
    myscript.js: line 2, col 19, Use '===' to compare with '0'.
    
    1 error
    $ ./node_modules/.bin/jshint --config cfg_jshint.json myscript.js 
    $

Users who experience any difference in this behavior are requested to file an
issue against this repository with more information.

## License

Copyright (c) 2017 Mike Pennisi  
Licensed under the MIT license.
