# simplelog

The simplest logging backend for [log](//github.com/carpentry-io/log) that
exists. Prints either to `stdout` or to `stderr`, depending on the log level.

## Example

```clojure
(load "git@github.com:carpentry-org/simplelog@0.0.2")

(defn main []
  (do
    (SimpleLog.install Log.DEBUG)
    (Log.trace "hi") ; will not be printed
    (Log.debug "hi again") ; will be printed to stdout
    (Log.warn "oops") ; will be printed to stderr
  )
)
```

<hr/>

Have fun!
