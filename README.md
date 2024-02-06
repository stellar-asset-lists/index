# Stellar Asset Lists Catalogue


## Ecosystem standard

SAL is a specification for lists of asset metadata that can be used by any Stellar applications and
services which rely on externally curated asset catalogs published by trusted providers.
This standard aims to enhance user experiences and trust by standardizing
a mechanism for defining, validating, and sharing curated lists of Stellar assets,
while ensuring ease of integration for wallets and applications across the Stellar network.

Any organization can create, maintain, and publish an asset list following the guidelines outlined
in the [SEP-42 standard](https://github.com/stellar/stellar-protocol/pull/1409).
Inclusion of any particular asset in a list should not be considered as endorsement or
recommendation.

This catalogue of asset lists is maintained by Stellar community developers.

## Use it in your application

The easiest way to utilize asset lists in your web app is a 
[@stellar-asset-lists/sdk](https://github.com/stellar-asset-lists/sdk) NPM package.

1. Fetch asset lists from the community-managed catalogue:
   ```js
   const catalogue = await fetchAvailableAssetLists()
   ```
2. Show available lists fetched from the catalogue to your users, so they could select one or more
lists from providers they trust. Save selected lists in user settings.

3. Load selected list on the client side and cache the result:
   ```js
   const list = await fetchAssetList('list_url')
   ```
4. Utilize a user-selected list to show only relevant assets in transfer/trade/swap interfaces.
This helps to combat various fraudulent schemes while delegating all the power of decision-making
to end-users in a truly decentralized manner.
5. Profit! Safer, more streamlined UX.

## Provide feedback

Have any thoughts how to improve the standard? Suggestions regarding a particular asset?
Complaints about the asset list provider?

Please leave your feedback [here](https://github.com/stellar-asset-lists/index/issues).

## Create your own asset list

If you want to become an asset list provider, please check 
[SEP-42 standard](https://github.com/stellar/stellar-protocol/pull/1409) specification,
prepare your list, make it publicly available, and create a
[ticket](https://github.com/stellar-asset-lists/index/issues).