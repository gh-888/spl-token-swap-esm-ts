```bash
$ pnpm install
$ npx tsc
```

Error:

```
node_modules/.pnpm/@solana+web3.js@1.75.0/node_modules/@solana/web3.js/lib/index.d.ts:6:28 - error TS7016: Could not find a declaration file for module 'node-fetch'. '/git/spl-token-swap-esm-ts/node_modules/.pnpm/node-fetch@2.6.9/node_modules/node-fetch/lib/index.js' implicitly has an 'any' type.
  Try `npm i --save-dev @types/node-fetch` if it exists or add a new declaration (.d.ts) file containing `declare module 'node-fetch';`

6 import * as nodeFetch from 'node-fetch';
                             ~~~~~~~~~~~~

src/index.ts:2:27 - error TS7016: Could not find a declaration file for module '@solana/spl-token-swap'. '/git/spl-token-swap-esm-ts/node_modules/.pnpm/@solana+spl-token-swap@0.2.1/node_modules/@solana/spl-token-swap/dist/esm/index.js' implicitly has an 'any' type.
  There are types at '/git/spl-token-swap-esm-ts/node_modules/@solana/spl-token-swap/dist/types/index.d.ts', but this result could not be resolved when respecting package.json "exports". The '@solana/spl-token-swap' library may need to update its package.json or typings.

2 import { TokenSwap } from "@solana/spl-token-swap";
                            ~~~~~~~~~~~~~~~~~~~~~~~~


Found 2 errors in 2 files.

Errors  Files
     1  node_modules/.pnpm/@solana+web3.js@1.75.0/node_modules/@solana/web3.js/lib/index.d.ts:6
     1  src/index.ts:2
```