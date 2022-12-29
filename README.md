```bash
git clone git@github.com:brillout/deno_vitejs-plugin-react-swc
cd deno_vitejs-plugin-react-swc/
deno task dev
```

Same as single line (copy-paste me):

```shell
git clone git@github.com:brillout/deno_vitejs-plugin-react-swc && cd deno_vitejs-plugin-react-swc/ && deno task dev
```

Go to [localhost:5173](http://localhost:5173/) and observe error:

```
11:32:40 AM [vite] Internal server error: Failed to convert napi value into rust type `Option<T>`
  Plugin: vite:react-swc
  File: /home/rom/tmp/deno_vitejs-plugin-react-swc/src/main.tsx
      at Compiler.<anonymous> (file:///home/rom/tmp/deno_vitejs-plugin-react-swc/node_modules/.deno/@swc+core@1.3.24/node_modules/@swc/core/index.js:216:33)
      at Generator.next (<anonymous>)
      at file:///home/rom/tmp/deno_vitejs-plugin-react-swc/node_modules/.deno/@swc+core@1.3.24/node_modules/@swc/core/index.js:34:71
      at new Promise (<anonymous>)
      at __awaiter (file:///home/rom/tmp/deno_vitejs-plugin-react-swc/node_modules/.deno/@swc+core@1.3.24/node_modules/@swc/core/index.js:30:12)
      at Compiler.transform (file:///home/rom/tmp/deno_vitejs-plugin-react-swc/node_modules/.deno/@swc+core@1.3.24/node_modules/@swc/core/index.js:202:16)
      at transform (file:///home/rom/tmp/deno_vitejs-plugin-react-swc/node_modules/.deno/@swc+core@1.3.24/node_modules/@swc/core/index.js:344:21)
      at TransformContext.transform (file:///home/rom/tmp/deno_vitejs-plugin-react-swc/node_modules/.deno/@vitejs+plugin-react-swc@3.0.1/node_modules/@vitejs/plugin-react-swc/index.mjs:42:24)
      at Object.transform (file:///home/rom/tmp/deno_vitejs-plugin-react-swc/node_modules/.deno/vite@4.0.3/node_modules/vite/dist/node/chunks/dep-0bae2027.js:41480:44)
      at async loadAndTransform (file:///home/rom/tmp/deno_vitejs-plugin-react-swc/node_modules/.deno/vite@4.0.3/node_modules/vite/dist/node/chunks/dep-0bae2027.js:39287:29)
```
