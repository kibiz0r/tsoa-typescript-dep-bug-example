# Demonstrates an issue with tsoa's typescript dependency

To exercise:

```
npm install -g typescript # need to install globally, since we'll be doing prod-only yarn install
yarn install --prod
yarn build
```

Should show an error:

```
yarn run v1.22.4
$ tsc
node_modules/@tsoa/runtime/dist/config.d.ts:1:21 - error TS2307: Cannot find module 'typescript' or its corresponding type declarations.

1 import * as ts from 'typescript';
                      ~~~~~~~~~~~~


Found 1 error.
```