##  Usage with Karma

karma.conf.js:

```
{
    var coverage: boolean;
    var reporters = [ 'kjhtml', 'mocha', 'notify' ];
    var preprocessors = ['webpack', 'sourcemap'];
    ...
    preprocessors: {
        'spec-bundle.js': coverage ? ['coverage'].concat(preprocessors) : preprocessors
    },
    ...
    webpack: getWebpackConfig(coverage),
    ...
    reporters: coverage ? ['coverage', 'junit'].concat(reporters) : reporters,
    browsers: [ coverage ? 'PhantomJS' : 'Chrome' ],
    ...    
```

note:
    Put your speaker notes here.
    You can see them pressing 's'.
