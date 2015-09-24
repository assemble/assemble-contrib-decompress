# grunt-assemble-decompress [![NPM version](https://badge.fury.io/js/grunt-assemble-decompress.svg)](http://badge.fury.io/js/grunt-assemble-decompress)

> Assemble plugin for extracting zip, tar and tar.gz archives.

```sh
$ npm i grunt-assemble-decompress --save
```

Next, add the plugin to the Assemble options:

```js
assemble: {
  options: {
    plugins: ['grunt-assemble-decompress', 'other/plugins/*.js']
  }
}
```

Visit the [plugins docs](http://assemble.io/plugins/) for more info about plugins or for help getting started.

## Options

## files

Type: `String`
Default: `undefined`

Path the file or files to decompress.

## dest

Type: `String`
Default: `undefined`

Destination for the decompressed files.

## Examples

```js
assemble: {
  options: {
    plugins: ['assemble-contrib-download', 'grunt-assemble-decompress'],
    download: {
      repo: 'assemble/handlebars-helpers',
      files: ['docs/helpers.zip'],
      dest: 'tmp/'
    }
    decompress: {
      files: ['tmp/helpers.zip'],
      dest: 'docs/helpers/'
    }
  }
}
```

## Other grunt-assemble plugins

* [grunt-assemble](https://www.npmjs.com/package/grunt-assemble): Static site generator for Grunt.js, Yeoman and Node.js. Used by Zurb Foundation, Zurb Ink, H5BP/Effeckt,… [more](https://www.npmjs.com/package/grunt-assemble) | [homepage](http://assemble.io)
* [grunt-assemble-anchors](https://www.npmjs.com/package/grunt-assemble-anchors): Assemble plugin for creating anchor tags from headings in generated html using Cheerio.js. | [homepage](https://github.com/assemble/grunt-assemble-anchors)
* [grunt-assemble-contextual](https://www.npmjs.com/package/grunt-assemble-contextual): Generates a JSON file with the context of each page. Basic plugin to help see… [more](https://www.npmjs.com/package/grunt-assemble-contextual) | [homepage](https://github.com/assemble/grunt-assemble-contextual)

## Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/assemble/grunt-assemble-decompress/issues/new).

## Author

**Jon Schlinkert**

+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License

Copyright © 2015 Jon Schlinkert
Released under the MIT license.

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on September 24, 2015._