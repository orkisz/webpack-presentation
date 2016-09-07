##  Webpack Hot Middleware

Webpack hot middleware allows you to add hot reloading into 
an existing server (e.g. Node.js Express).
It comes pretty handy if you have dummy API 
in your Express and you want to use it with front-end 
application on the same port.
  
  Sample usage (Express server part):
  ```
  
  var webpack = require('webpack');
  var webpackConfig = require('./webpack.config');
  var compiler = webpack(webpackConfig);
  
  app.use(require("webpack-dev-middleware")(compiler, {
      noInfo: true, publicPath: webpackConfig.output.publicPath
  }));
  ```
  
  Then you should add webpack-hot-middleware as
  a plugin and connect it in your webpack config as an entry.
