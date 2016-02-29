# ignore file loader for webpack

You just want the url of the resource but not the output!

This plugin is ideal for isomorphic apps where you don't care about the images in the server-side app, because you already have a client-side app that optimizes the images.

## Usage

[Documentation: Using loaders](http://webpack.github.io/docs/using-loaders.html)

``` javascript
var url = require("ignore-file!./file.png");
// => does NOT emits file.png as file in the output directory and returns the public url
// => returns i. e. "/public-path/0dcbbaa701328a3c262cfd45869e351f.png"
```

By default the filename of the resulting file is the MD5 hash of the file's contents
with the original extension of the required resource.

## License

MIT (http://www.opensource.org/licenses/mit-license.php)
