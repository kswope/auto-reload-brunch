# auto-reload-brunch-express

Fork of auto-reload-brunch that adds the functionality of running an express
server with 'hot reloading' and browser reloading.  In other words, you don't
need nodemon and the browser is refreshed automatically.

Be sure to run brunch without --server option

Additional configs for brunch-config.js (also activates running of express)
``` js

module.exports = {
  ...
  plugins: {
    autoReload: {
      app: {
        reloadBrowser: true,
        path: './app.js',
        port: 3000,
        watch: [ 'routes', 'views' ]
      }
    }
  },
  ...
}


```

See the [original](https://github.com/brunch/auto-reload-brunch) for more and better info

## License

The MIT License (MIT)

Copyright (c) 2012-2017 Paul Miller (http://paulmillr.com)

Copyright (c) 2017 Kevin Swope <github-kevdev@snkmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

<!-- References -->

[brunch]: http://brunch.io
[anymatch]: https://www.npmjs.com/package/anymatch
