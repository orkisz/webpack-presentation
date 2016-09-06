##  Configuration - Resolve

Controls how files are resolved with *require* method

```
resolve: {
      extensions: Array<string>, // ['', '.ts', '.js', '.json'],
      root: string, // usually absolute path to './src'
      modulesDirectories: Array<string> // ['node_modules'],
      alias: {
            'my-module': './src/app/module1/.../my-module.ts' // nice way to simplify imports
      }
}
```

note:
    Put your speaker notes here.
    You can see them pressing 's'.
