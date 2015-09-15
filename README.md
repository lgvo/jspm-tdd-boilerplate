# jspm-tdd-boilerplate
A Boilerplate to use JSPM / Babel / Karma / Mocha / Chai.


Create your site and libs with ES6, with tests.

## Setup

```bash
npm install

jspm install

karma start # will watch for file changes and automatic run all tests
```

## Config

By the default all Javascript are supposed to be in 'app/' also the tests.
To change that you just need to set the pattern that karma will look for, at the 'karma.conf.js' file.

``` javascript
// ...

    jspm: {
        loadFiles: ['your_test_folder/**/*.spec.js'], // he are the files that are loaded automatic (test files)
        serveFiles: ['your_app_folder/**/!(*.spec).js'] // he are the files that are loaded with import statement
    },

// ...
```

### License

[MIT](LICENSE)

