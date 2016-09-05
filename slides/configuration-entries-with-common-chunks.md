##  Configuration - Entries with Common Chunks

Webpack can split application into several independent parts and save common code into **common chunks**

For e.g. large app can load its main part on start, but less-used modules will be loaded asynchronously on-demand

```
'main':      './src/app.ts' // app starting point
'module2':   './src/not-often-used-module/xxx.ts'
```

If those two entries have common code (like components) they will go into **common chunks** thanks to `CommonChunksPlugin`

note:
    Put your speaker notes here.
    You can see them pressing 's'.
