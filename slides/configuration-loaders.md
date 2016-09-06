##  Configuration - Loaders

```
(pre|post)loaders: [
    {
        test: Regexp, // A condition that must be met
        exclude: Array<Regexp>, // A condition that must not be met
        include: Array<Regexp>, // A condition that must be met
        loader: string, // A string of “!” separated loaders
        loaders: Array<string>, // An array of loaders as string,
        query: Object // Only when there is one loader
    }
]
```

Example

```
{
    test: /\.ts$/,
    loader: awesome-typescript-loader?tsconfig=tsconfig.json!angular2-template-loader,
    exclude: [
        /\.e2e\.ts$/,
        /\.spec\.ts$/
    ]
}
```

note:
    "loader" and "loaders" are mutually exclusive
