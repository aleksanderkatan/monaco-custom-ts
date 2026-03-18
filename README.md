# monaco-custom-ts

A fork of [microsoft/monaco-editor](https://github.com/microsoft/monaco-editor)
meant for swapping the TypeScript instance used by Monaco.

## Usage

### Option A: Prebuilt with `tsover`

A prebuilt Monaco with [tsover](https://github.com/software-mansion-labs/tsover)
will be available on NPM in near future.

### Option B: Build locally

Clone the repo, replace TypeScript version and build (substitute
`npm:tsover@^5.9.11` with the desired version):

```sh
npm install -D "typescript@npm:tsover@^5.9.11" && npm install && npm run import-typescript && npm run build
```

Then in your project's `package.json`, link an appropriate path, for example:

```json
"monaco-editor": "file:../monaco-custom-ts/out/monaco-editor"
```
