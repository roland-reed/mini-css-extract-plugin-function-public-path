# Reproduce steps

- `pnpm i`
- `pnpx webpack`

The following errors are expected:

```plain
assets by status 822 bytes [cached] 1 asset
runtime modules 663 bytes 3 modules
cacheable modules 71 bytes
  ./src/index.js 32 bytes [built] [code generated]
  ./src/index.css 39 bytes [built] [code generated] [1 error]

ERROR in ./src/index.css
Module build failed (from ./node_modules/.pnpm/mini-css-extract-plugin@2.4.5_webpack@5.64.4/node_modules/mini-css-extract-plugin/dist/loader.js):
TypeError: publicPath.replace is not a function
    at Object.pitch (/Users/username/Workspace/test/webpack-demo/node_modules/.pnpm/mini-css-extract-plugin@2.4.5_webpack@5.64.4/node_modules/mini-css-extract-plugin/dist/loader.js:176:114)
 @ ./src/index.js 1:0-21

webpack 5.64.4 compiled with 1 error in 285 ms
```
