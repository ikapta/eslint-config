# `@kapta/eslint-config-ts`

> eslint + prettier

## Setup

```shell
yarn add -D @kapta/eslint-config-ts
```

## Usage

config `.eslintrc.js`

```js
module.exports = {
  "extends": "@kapta/eslint-config-ts",
  parserOptions: {
    project: './tsconfig.json',
  },
};
```

config `.prettierrc.js`

```tsx
module.exports = require('@kapta/eslint-config-ts/prettier.config');
```

config `package.json` scripts:

```json
 "scripts": {
   "lint": "eslint *.ts src test",
   "lint:fix": "eslint --fix *.ts src test xxx"
}
```
