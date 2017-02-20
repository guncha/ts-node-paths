# ts-node-paths

```sh
# works
$ ./node_modules/.bin/tsc --noEmit --project lib
```

```sh
# doesn't work
$ ./node_modules/.bin/ts-node --project lib lib/print_hello.ts
Error: Cannot find module 'lib/dep'
    at Function.Module._resolveFilename (module.js:440:15)
    at Function.Module._load (module.js:388:25)
    at Module.require (module.js:468:17)
    at require (internal/module.js:20:19)
    at Object.<anonymous> (/Users/gunca/Code/ts-node-paths/lib/print_hello.ts:1:1)
    at Module._compile (module.js:541:32)
    at Module.m._compile (/Users/gunca/Code/ts-node-paths/node_modules/ts-node/src/index.ts:413:23)
    at Module._extensions..js (module.js:550:10)
    at Object.require.extensions.(anonymous function) [as .ts] (/Users/gunca/Code/ts-node-paths/node_modules/ts-node/src/index.ts:416:12)
    at Module.load (module.js:458:32)
```
