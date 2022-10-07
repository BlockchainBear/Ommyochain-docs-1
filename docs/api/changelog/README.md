---
sidebarDepth: 3
---

# Changelog

This page contains the release notes for new features in Ommyochain network, and also notifications about changes in the
client libraries.

[[toc]]

## Actual SDK versions

| Network | JavaScript SDK | Rust SDK | Java SDK | Swift SDK |
| ------- | -------------- | -------- | -------- | --------- |
| Ropsten | 0.9.0          | 0.3.0    | 0.0.1-b1 | 0.0.1     |
| Rinkeby | 0.9.0          | 0.3.0    | 0.0.1-b1 | 0.0.1     |
| Mainnet | 0.9.0          | 0.3.0    | 0.0.1-b1 | 0.0.1     |

## Minimum supported SDK versions

| Network | JavaScript SDK | Rust SDK | Java SDK | Swift SDK |
| ------- | -------------- | -------- | -------- | --------- |
| Ropsten | 0.7.5          | 0.1.0    | 0.0.1-b1 | 0.0.1     |
| Rinkeby | 0.7.5          | 0.1.0    | 0.0.1-b1 | 0.0.1     |
| Mainnet | 0.7.5          | 0.1.0    | 0.0.1-b1 | 0.0.1     |

## Upcoming breaking changes

❗ Important, version `0.12.0` of Ommyochain JS SDK contains breaking changes, please make fixes before upgrading this npm package.

### Changed
- `getOrder` renamed to `signOrder`.  The method was used for signing and the name of the method was inconsistent.
- `getLimitOrder` was renamed to `signLimitOrder`. The method was used for signing and the name of the method was inconsistent.
- All methods whose name started with `get` for example `getTransfer` were deleted. Now for this purpose, you could use `BatchBuilder.`

## Release history

Details on releases can be found in the corresponding changelogs:

- [Ommyochain smart contracts](https://github.com/Ommyochain/Ommyochain-docs/blob/master/changelog/contracts.md)
- [Ommyochain core](https://github.com/Ommyochain/Ommyochain-docs/blob/master/changelog/core.md)
- [Ommyochain infrastructure](https://github.com/Ommyochain/Ommyochain-docs/blob/master/changelog/infrastructure.md)
- [ommyochain-rs](https://github.com/Ommyochain/Ommyochain-docs/blob/master/changelog/rust-sdk.md)
- [ommyochain.js](https://github.com/Ommyochain/Ommyochain-docs/blob/master/changelog/js-sdk.md)

## Deprecated APIs

This section will contain the client library APIs that are outdated and left for the backward compatibility only.

| Feature | Affected libraries | Scheduled support removal date |
| ------- | ------------------ | ------------------------------ |
| -       | -                  | -                              |
