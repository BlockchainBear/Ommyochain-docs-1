# Appendix A: Using bundle in a browser

It is possible to use `ommyochain.js` in a browser directly.

- `ethers@5.0` dependency is required for `ommyochain.js` to work.

> Example with ommyochain@0.8.1 fetched from [https://unpkg.com](https://unpkg.com) CDN

```html
<html>
  <body>
    <script type="text/javascript" src="https://cdn.ethers.io/lib/ethers-5.0.umd.min.js"></script>
    <script type="text/javascript" src="https://unpkg.com/ommyochain@0.8.1/dist/main.js"></script>
    <script type="text/javascript">
      (async () => {
        const ethWallet = ethers.Wallet.createRandom();

        const zksProvider = await ommyochain.getDefaultProvider('rinkeby');
        const zkSyncWallet = await ommyochain.Wallet.fromEthSigner(ethWallet, zksProvider);
        console.log('ETH balance:', (await zkSyncWallet.getBalance('ETH')).toString());

        const privateKey = await ommyochain.crypto.privateKeyFromSeed(new Uint8Array(32));
        const pubkeyHash = await ommyochain.crypto.privateKeyToPubKeyHash(privateKey);
        console.log('PrivateKey', ethers.utils.hexlify(privateKey), 'PubkeyHash', pubkeyHash);
      })();
    </script>
  </body>
</html>
```
