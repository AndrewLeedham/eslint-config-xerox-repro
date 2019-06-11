# eslint-config-xerox-repro

Highlights an issue with eslint-plugin-jsdoc and async function with and without TypeScript.

## The following errors occur:
```
Andrews-MacBook-Pro:eslint-plugin-jsdoc andrew$ yarn lint:js
yarn run v1.15.2
$ eslint ./src --ext .js --config ./.eslintrc.js.json

/Users/andrew/Documents/GitHub/Repro/eslint-plugin-jsdoc/src/index.js
  1:1  error  Missing JSDoc @returns declaration  jsdoc/require-returns

✖ 1 problem (1 error, 0 warnings)

error Command failed with exit code 1.
info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.
Andrews-MacBook-Pro:eslint-plugin-jsdoc andrew$ yarn lint:ts
yarn run v1.15.2
$ eslint ./src --ext .ts --config ./.eslintrc.ts.json

/Users/andrew/Documents/GitHub/Repro/eslint-plugin-jsdoc/src/index.ts
  1:1  error  Missing JSDoc @returns declaration  jsdoc/require-returns

✖ 1 problem (1 error, 0 warnings)

error Command failed with exit code 1.
```

## Expected Behaviour:
No errors.