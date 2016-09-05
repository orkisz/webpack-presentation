##  What is a Loader

* It’s a node module that exports one function
* Function recieve a content parameter
    * File content if loader is first
    * Result from prevoius loader
* Function can finish its job in several ways
    * Just return content
    * Invoke `this.callback(err, result[, additionalResults])`
    * Switch into async mode `var callback = this.async()` and then finish async operation with `callback(err, result[, additionalResults])`

