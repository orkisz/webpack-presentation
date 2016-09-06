##  Configuration - Externals

Externals allow to mark some module as external - this means it won't be resolved at compilation but rather at runtime.

```
externals: [
    'moment': 'window.moment', // all moment calls will be linked to window.moment global object
    'lodash': 'window._',
    'React': 'React',
    ...
]
```

and in index.html:

```
<script src="https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.14.1/moment-with-locales.min.js"></script>
...
```

note:
    Put your speaker notes here.
    You can see them pressing 's'.
