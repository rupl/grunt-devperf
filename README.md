# grunt-devperf

> Helps front-end developers to maintain a good quality, based on phantomas and grunt-phantomas.

## Getting Started
This plugin requires Grunt `~0.4.4`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-devperf --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-devperf');
```

## The "devperf" task

### Overview
In your project's Gruntfile, add a section named `devperf` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  devperf: {
    options: {
      urls: [
        'http://www.google.com'
      ]
    }
  }
});
```

### Options

#### options.urls
Type: `Array of Strings`
Default value: `'http://www.google.fr'`

The list of URLs you want to test


### Usage Examples

In this example, several Urls are tested

```js
grunt.initConfig({
  devperf: {
    options: {
      urls: [
        'http://www.france2.fr',
        'http://www.france3.fr',
        'http://www.france4.fr',
        'http://www.france5.fr'
        'http://www.franceo.fr'
      ]
    }
  }
});
```
Then, open the /devperf/index.html file with your browser to see the results.

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
_Initial commit_