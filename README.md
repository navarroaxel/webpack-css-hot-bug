# webpack-css-hot-bug

This repo exists to show a css-hot-loader bug in webpack@4.

## Related issues

https://github.com/shepherdwind/css-hot-loader/issues/37

## Reproducing the bug
After clone this repo you should run the following commands:

    yarn install
    yarn start

Open http://localhost:3000 and you can see the TypeError on the console of the DevTools when the page loads the `main.bundle.js`.

The error is fixed in the bundle when a hot change is made to the SCSS file and the bundle is reloaded.
