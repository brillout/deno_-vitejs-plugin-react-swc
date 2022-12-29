```bash
git clone git@github.com:brillout/deno_vitejs-plugin-react-swc
cd deno_vitejs-plugin-react-swc/
deno task dev
```

Same as single line (copy-paste me):

```shell
git clone git@github.com:brillout/deno_vitejs-plugin-react-swc && cd deno_vitejs-plugin-react-swc/ && deno task dev
```

Observe error:

```
Task dev deno run -A --unstable --node-modules-dir npm:vite
failed to load config from /home/rom/tmp/vite-project/vite.config.mts
error when starting dev server:
TypeError: Failed caching npm package '@swc/core-darwin-arm64@1.3.24'.
    at async loadConfigFromBundledFile (file:///home/rom/tmp/vite-project/node_modules/.deno/vite@4.0.3/node_modules/vite/dist/node/chunks/dep-0bae2027.js:62058:21)
    at async loadConfigFromFile (file:///home/rom/tmp/vite-project/node_modules/.deno/vite@4.0.3/node_modules/vite/dist/node/chunks/dep-0bae2027.js:61943:28)
    at async resolveConfig (file:///home/rom/tmp/vite-project/node_modules/.deno/vite@4.0.3/node_modules/vite/dist/node/chunks/dep-0bae2027.js:61564:28)
    at async createServer (file:///home/rom/tmp/vite-project/node_modules/.deno/vite@4.0.3/node_modules/vite/dist/node/chunks/dep-0bae2027.js:60884:20)
    at async CAC.<anonymous> (file:///home/rom/tmp/vite-project/node_modules/.deno/vite@4.0.3/node_modules/vite/dist/node/cli.js:729:24)
```
