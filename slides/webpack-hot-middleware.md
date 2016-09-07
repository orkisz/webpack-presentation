##  Webpack Dev Middleware

Webpack dev middleware allows you to add local server feature to 
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
  
