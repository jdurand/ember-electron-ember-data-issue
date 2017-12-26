# ember-electron + ember-data issue

[ember-electron issue #332](https://github.com/felixrieseberg/ember-electron/issues/332)

### Steps to reproduce :

- `git clone https://github.com/jdurand/ember-electron-ember-data-issue.git`
- `cd ember-electron-ember-data-issue`
- `npm i && ember electron:package -e production`
- `open electron-out/ember-electron-issue-darwin-x64/ember-electron-issue.app`

In the console, you should get something like `Uncaught ReferrenceError: a22500 is not defined`

Note that if you either `npm uninstall ember-data` or package in development `ember electron:package -e development` this error is not thrown.
