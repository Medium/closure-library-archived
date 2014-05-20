# Closure Library [![Build Status](https://travis-ci.org/google/closure-library.svg?branch=master)](https://travis-ci.org/google/closure-library)

This is Medium's fork of the
[Google Closure Library](https://github.com/google/closure-library).

We try to keep it reasonably up to date, but only after testing that it is
compatible with our products. There may occasionally be changes introduced to
work around temporary issues or to try out fixes in preparation of upstream
patches.

The package number reflects the date that we last merged the fork. We rebase
our changes on top of origin/master, so that our modifications are always on top of
the closure-library master changes.
gi
## Merging from the main project

The 'pristine' branch contains only changes that we've pulled from the main repo.

The 'master' branch should always contain main repo changes, with our changes layered on top.

To sync changes from the main project, run the following:

```
# Sync changes from code.google.com
git clone git@github.com:Obvious/closure-library
cd closure-library
git remote add google git@github.com:google/closure-library
git fetch google
git checkout pristine
git merge google/master
git push origin pristine

# Layer our changes on top
git checkout master
git rebase pristine master
```

## NPM Info

The repository contains a lot of test files and demos, as such we include a
postinstall script that removes these files from the `node_modules` directory
when installed via NPM.

## Contributing

This project isn't intended for external contribution, we suggest instead you
[send patches](https://code.google.com/p/closure-library/wiki/Contributors)
directly.

## Original Readme

Closure Library is a powerful, low-level JavaScript library designed
for building complex and scalable web applications. It is used by many
Google web applications, such as Google Search, Gmail, Google Docs,
Google+, Google Maps, and others.

For more information, visit the
[Google Developers](https://developers.google.com/closure/library) or
[GitHub](https://github.com/google/closure-library) sites.

Download the latest stable version on our [releases page](https://github.com/google/closure-library/releases).

Developers, please see the
[Generated API Documentation](https://google.github.io/closure-library/api/).

See also the
[goog.ui Demos](https://google.github.io/closure-library/source/closure/goog/demos/)

## Using with Node.js
Install the [official package](https://www.npmjs.com/package/google-closure-library) from npm.

```
npm install google-closure-library
```

Require the package and use goog.require normally.

```
require("google-closure-library");

goog.require("goog.crypt.Sha1");

var sha1 = new goog.crypt.Sha1();
sha1.update("foobar");
var hash = sha1.digest();
```
