# monaco-custom-ts

A fork of [microsoft/monaco-editor](https://github.com/microsoft/monaco-editor)
meant for swapping the TypeScript instance used by Monaco.

## Usage

### Option A: Prebuilt (tsover)

A prebuilt Monaco with [tsover](https://github.com/software-mansion-labs/tsover)
is available on the `tsover` branch. In your project's `package.json`, add:

```json
"monaco-editor": "github:aleksanderkatan/monaco-custom-ts#tsover"
```

### Option B: Build locally

Clone the repo, replace TypeScript version and build (substitute
`npm:tsover@^5.9.11` with the desired version):

```sh
npm install -D "typescript@npm:tsover@^5.9.11" && npm run build
```

Then in your project's `package.json`, link an appropriate path, for example:

```json
"monaco-editor": "file:../monaco-custom-ts/out/monaco-editor"
```
