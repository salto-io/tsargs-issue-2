# Reproduction for TypeScript compilation issue in tsargs

## [Issue](https://github.com/Morglod/tsargs/issues/2)

When the TypeScript `noUnusedParameters` option is set, errors like these are emitted:

```text
node_modules/tsargs/lib/pre-argn.ts:261:316 - error TS6133: 'J' is declared but its value is never read.
```

## To reproduce

```bash
  yarn
```

For the compilation to work, comment out the `noUnusedParameters` option in the `tsconfig.json` file.
