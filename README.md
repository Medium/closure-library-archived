# Closure Library [![Build Status](https://travis-ci.org/google/closure-library.svg?branch=master)](https://travis-ci.org/google/closure-library)

This is Medium's fork of the
[Google Closure Library](https://github.com/google/closure-library).

The Closure project was started in 2006 in a very different browser landscape to
today. Browsers were rapidly changing yet upgrade cycles were still slow. Closure
provided a common abstraction layer that accounted for the myriad of differences
and bugs.

It is Medium's intent to modernize Closure. We consider it the missing standard
library for JavaScript, and will evolve it to match that description. We will be
removing old browser compatibility code and much of the UI features. We will work
with the Closure Compiler and Templates teams, as compatibility there is important
to us.

The version of the upstream Closure Library that we are working from will always
be available in origin/pristine.

## Using

```
require('obvious-closure-library').bootstrap()
goog.require('goog.string.linkify')
goog.string.linkify.linkifyPlainText('Hello www.world.com')
```

## NPM Info

The repository contains a lot of test files and demos, as such we include a
postinstall script that removes these files from the `node_modules` directory
when installed via NPM.

## Contributing

Currently, this project isn't intended for external contribution, we suggest
instead you [send patches](https://code.google.com/p/closure-library/wiki/Contributors)
directly.

## Original Readme

Closure Library is a powerful, low-level JavaScript library designed
for building complex and scalable web applications. It is used by many
Google web applications, such as Google Search, Gmail, Google Docs,
Google+, Google Maps, and others.

For more information, visit the
[Google Developers](https://developers.google.com/closure/library) or
[GitHub](https://github.com/google/closure-library) sites.

Developers, please see the
[Generated API Documentation](http://google.github.io/closure-library/api/).

See also the
[goog.ui Demos](http://google.github.io/closure-library/source/closure/goog/demos/)

