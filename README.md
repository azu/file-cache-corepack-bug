## Setup

    corepack enable npm
    npm install

## Test

without npx

    npm test

with npx 

    npm run test-npx
    
## Bug

Node 16 + packageManager: npm@6.14.16 + corepack has a bug.

Throw next error on `npm run test-npx`

    TypeError: Invalid host defined options
    
    or 
    
    TypeError [ERR_VM_DYNAMIC_IMPORT_CALLBACK_MISSING]: A dynamic import callback was not specified.


## Workaround

Use `node_modules/.bin/create-validator-ts` instead of `npx create-validator-ts`.
