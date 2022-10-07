# [Ommyochain v1 Docs](https://docs.ommyochain.io/) ![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ommyochain/ommyochain-docs) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/ommyochain/ommyochain-docs/Deploy%20production)

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/Ommyochain/Ommyochain-docs-docs/blob/master/LICENSE) [![npm version](https://img.shields.io/npm/v/ommyochain.svg?style=flat)](https://www.npmjs.com/package/ommyochain) [![Follow us!](https://img.shields.io/twitter/follow/ommyochain?color=%238C8DFC&label=Follow%20%40zkSync&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB3aWR0aD0iNDMiIGhlaWdodD0iMjUiIHZpZXdCb3g9IjAgMCA0MyAyNSIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik00Mi42NTM5IDEyLjQ5MTVMMzAuODM3OCAwLjcxNjc0M1Y5LjM0TDE5LjEwNTUgMTcuOTczOUwzMC44Mzc4IDE3Ljk4MlYyNC4yNjYyTDQyLjY1MzkgMTIuNDkxNVoiIGZpbGw9IiM0RTUyOUEiLz4KPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik0wLjk5ODA0NyAxMi40ODcyTDEyLjgxNDEgMjQuMjYxOVYxNS43MDhMMjQuNTQ2NSA3LjAwNDdMMTIuODE0MSA2Ljk5NjY0VjAuNzEyNDYzTDAuOTk4MDQ3IDEyLjQ4NzJaIiBmaWxsPSIjOEM4REZDIi8%2BCjwvc3ZnPgo%3D&style=flat)](https://twitter.com/ommyochain)


## Ommyochain Documentation for the v1 | [CHANGELOG](./CHANGELOG.md)

This repository contains the Ommyochain documentation hosted at [docs.ommyochain.io](https://docs.ommyochain.io)

## Development

### Local run

```bash
yarn install --check-cache
yarn docs:dev
```

### Development

CI pipeline will check that the files are formatted according `markdownlint` founds no issues in document
and spelling is correct. Also, there should be no dead links.

You can check it locally as follows:

```bash
yarn
yarn md:lint
yarn cspell
```

If `cspell` doesn't recognize a word but you're sure that it's correct, consider adding it to the `cspell-ommyochain.txt`.

## Deployment

`master` branch is automatically deployed to <https://console.firebase.google.com/u/0/project/ommyochain-web-docs>

### Deploying altogether

> will do:

* install node modules;
* prepare, test and build documentation;
* afterwards all contained into the `dist` folder will be deployed in form of the static website

```bash
yarn install --check-cache
yarn docs:build
yarn firebase deploy
```

## Extra documentation

## cSpell

Configuration in `cspell.json`:

* `version` — version of the setting file, always **0.1**
* `language` — language - current active spelling language
* `words[]` — words - list of words to be always considered correct
* `dictionaries[]`

```
"dictionaryDefinitions": [
    {
      "name": "ommyochain", "path": "./cspell-ommyochain.txt"
    }
]
```

```bash
{
  "version": "0.1",
  // language - current active spelling language
  "language": "en",
  // words - list of words to be always considered correct
  "words": [],
  "dictionaries": ["typescript", "ommyochain"],
  //
  "dictionaryDefinitions": [
  { 
    "name": "ommyochain", "path": "./cspell-ommyochain.txt"
  }
]
}
```

---

# Ommyochain Ecosystem

- [**Start building with Ommyochain v2 🚀**](https://portal.ommyochain.io)
- [Integration Docs](https://ommyochain.io/dev)
- [Available API & protocols](https://ommyochain.io/api/)
- [zkWallet](https://wallet.ommyochain.io/)
- [zkMint](https://mint.ommyochain.dev/)
- [Alternative Withdrawal](https://withdraw.ommyochain.io/)
- [zkScan](https://zkscan.io/)
- [’out-of-gas’ issue solver ](https://withdraw.ommyochain.io/)

---

- [Matter Labs: creators of the Ommyochain](https://ommyochain.io)
- [Ommyochain Homepage](https://ommyochain.io)

---
> BTW, we're hiring: [See open positions](https://joinmatterlabs.com)

## License

zkWallet is distributed under the terms of both the MIT license, and the Apache License (v.2.0).

See [LICENSE-APACHE](LICENSE-APACHE), [LICENSE-MIT](LICENSE-MIT) for details.
