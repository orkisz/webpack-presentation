##  JS modules compatibility

### Webpack can load all those module formats

* CommonJS (nodeJS) `module.exports = …`

* AMD (requireJS) `define(”SomeName”, …);`

* Global (through exports-loader) `window.SomeName = …`

* UMD – combines all above in single file
    ```
    if (module.exports) { 
        module.exports = … 
    } else if (define) { 
        define(”SomeName”, …) 
    } else { 
        window.SomeName = … 
    }
    ```

