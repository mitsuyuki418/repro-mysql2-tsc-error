# repro-mysql2-tsc-error

A repro code for
https://github.com/sidorares/node-mysql2/issues/2086

```bash
npm install
```

Then,

```bash
npx tsc
```

it shows the following errors, because the mysql2 3.4.1 contains not only d.ts files but also ts files.

```
Errors  Files
     3  node_modules/mysql2/typings/mysql/lib/protocol/sequences/ExecutableBase.ts:84
     3  node_modules/mysql2/typings/mysql/lib/protocol/sequences/promise/ExecutableBase.ts:62
     3  node_modules/mysql2/typings/mysql/lib/protocol/sequences/promise/QueryableBase.ts:62
     3  node_modules/mysql2/typings/mysql/lib/protocol/sequences/QueryableBase.ts:84
```
