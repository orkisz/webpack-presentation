##  Loaders

#### Loaders do main processing of source files. By default it means compiling them to output format (for code/styles)

* Compile TS/TSX/ES6/ES7/JSX code to ES5
* Transform SASS/SCSS/LESS into CSS
* Export various types of templates (HTML, JADE, Reactive templates, Markdown)
* Process images:
    * If size larger than x bytes, copy them to output folder and fix reference
    * If size smaller than x bytes, inline them in JS/CSS as byte64-encoded string
