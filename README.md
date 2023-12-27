# Nuxt 3 + @antfu/eslint-config

Minimal demo project for reproducing an eslint error:

> Cannot write file '~/eslint.config.js' because it would overwrite input file.

![Screenshot](https://i.postimg.cc/NfnT5f5R/Screenshot-2023-12-27-at-11-12-18.png)

Step to reproduce an error:
- Clone the project and install dependencies
```bash
git clone https://github.com/juretopolak/nuxt-antfu-eslint.git
cd nuxt-antfu-eslint
pnpm i
pnpm dev
```
- Open the file ./server/api/test.get.ts with VSCode
- TS error appear in ./server/tsconfig.json

**Error only appears when any file in the ./server directory is opened!**
