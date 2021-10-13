# SDK Packages

[![Logo](https://raw.githubusercontent.com/gnosis/safe-apps-sdk/master/assets/logo.png)](https://gnosis.pm/) [![Build Status](https://camo.githubusercontent.com/16e0d52abc7d0686cc97ffa341d0fbc5b1704440b6d5835e566a956ebd8835e2/68747470733a2f2f7472617669732d63692e6f72672f676e6f7369732f736166652d617070732d73646b2e7376673f6272616e63683d6d6173746572)](https://travis-ci.org/gnosis/pm-contracts)

Components library

Developer tools to integrate third-party applications \(Safe Apps\) with Safe Multisig \([https://gnosis-safe.io/app/](https://gnosis-safe.io/app/)\).

Import Docs from Github repo

You can find more resources on Safe Apps in the [Gnosis Safe Developer Portal](https://docs.gnosis.io/safe/docs/sdks_safe_apps/).

[![safeapps\_pathways\_v4](https://user-images.githubusercontent.com/6764315/123075714-c5564100-d418-11eb-8da0-898aa163dee2.png)](https://user-images.githubusercontent.com/6764315/123075714-c5564100-d418-11eb-8da0-898aa163dee2.png)

## Packages

| Package | Description |
| :--- | :--- |
| [cra-template-safe-app](https://github.com/gnosis/safe-apps-sdk/tree/master/packages/cra-template-safe-app) | CRA template to quickly bootstrap a Safe app |
| [safe-apps-react-sdk](https://github.com/gnosis/safe-apps-sdk/tree/master/packages/safe-apps-react-sdk) | A wrapper of safe-apps-sdk with helpful hooks |
| [safe-apps-sdk](https://github.com/gnosis/safe-apps-sdk/tree/master/packages/safe-apps-sdk) | JavaScript SDK |
| [safe-apps-provider](https://github.com/gnosis/safe-apps-sdk/tree/master/packages/safe-apps-provider) | A generic provider that can be used with common web3 libraries |
| [safe-apps-onboard](https://docs.blocknative.com/onboard) | Blocknative included Safe App support in onboard.js v1.26.0. To use it, add `{ walletName: "gnosis" }` to wallet list. |
| [safe-apps-web3modal](https://github.com/gnosis/safe-apps-sdk/tree/master/packages/safe-apps-web3modal) | A wrapper around Web3modal that would automatically connect to the Safe if the app is loaded as a Safe app |
| [safe-apps-web3-react](https://github.com/gnosis/safe-apps-sdk/tree/master/packages/safe-apps-web3-react) | A web-react connector for Safe Apps |

## Testing your Safe App

You can use any of our production interfaces:

* Mainnet: [https://gnosis-safe.io](https://gnosis-safe.io/)
* Rinkeby: [https://rinkeby.gnosis-safe.io](https://rinkeby.gnosis-safe.io/)
* xDai: [https://xdai.gnosis-safe.io](https://xdai.gnosis-safe.io/)

We also made a very simple interface for testing safe apps that can be used on any network: [https://dev.gnosis-safe.io/](https://dev.gnosis-safe.io/)

## Setting up development environment

### Installing dependencies

```text
npm i -g lerna
yarn global add lerna

lerna bootstrap
```

### Running commands

We will use `build` command as an example. Same applies to other commands.

For all packages:

```text
lerna run build
```

For a specific package:

```text
lerna run --scope @gnosis.pm/safe-apps-sdk build --stream
```

`--stream` options enables command output. By default, lerna displays it only in case of an error.


