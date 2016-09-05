##  Webpack Dev Server Features

* Live reload
    * Iframe mode – Page is loaded in iframe and refreshed on a change
    * Inline mode – Little JS script responsible for refreshing is added to the bundle 
* HMR – Hot Module Replacement
* Proxy – You can have local assets but still use external backend API. Proxy will translate local URL to remote one (or local, on a different host).

note:
    Please remember that some IDEs have safe write feature enabled by default. IDE is saving temp file before saving an actual file. With this option, autorefresh obviously won’t work.
