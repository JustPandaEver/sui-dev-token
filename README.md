# sui-dev-token

Fake Token on Sui Devnet for Testing Only

## Publish

Run
`sui client publish  --gas-budget 10000`

### Result

```
Created Objects:
  - ID: 0x2009591841eff19d6c5e97eae7a45f2f3908e502 , Owner: Immutable
  - ID: 0x569832dd430ea3d31853b2e93e545bde89526021 , Owner: Shared
  - ID: 0x86d252653e78b9f7c7b5382f93f5c74852544e1c , Owner: Shared
  - ID: 0x88aa89fa8f405223401e212548798965655ac189 , Owner: Immutable
  - ID: 0xd5805a9e4037ef5ae51afbab2a4cd36090bb6c8a , Owner: Immutable
  - ID: 0xd5c1f62d32f140a59c2ce2997a912b1bd43623a1 , Owner: Immutable
  - ID: 0xde87ddc6cc6570ae8ff3bf9ab4cf07b2d5f7bba3 , Owner: Shared
```

### Package
0x2009591841eff19d6c5e97eae7a45f2f3908e502

### CoinMetadata
* BTC: 0xd5c1f62d32f140a59c2ce2997a912b1bd43623a1
* ETH: 0x88aa89fa8f405223401e212548798965655ac189
* SUI: 0xd5805a9e4037ef5ae51afbab2a4cd36090bb6c8a


### Registry
* BTC: 0x86d252653e78b9f7c7b5382f93f5c74852544e1c
* ETH: 0x569832dd430ea3d31853b2e93e545bde89526021
* SUI: 0xde87ddc6cc6570ae8ff3bf9ab4cf07b2d5f7bba3


## Usage (Updated)

```
export TOKEN_PACKAGE=0xc6e0ac81e9640d3afdc8a1b77c16e9aaecd4ed3c
export BTC=0x57dc4685653ca1265aa36524ffe318ce86cd1827
export ETH=0x4b234973f74d88933d2f4bedf4fb755fa9255dec
export SUI=0x503791addd188e97484ffd28565bfaf75c6749cd
export USDC=0x4d5c08a8d253c84d21e253dda525f651be04a8c2
```

### Mint BTC
`sui client call --gas-budget 10000 --package $TOKEN_PACKAGE --module "btc" --function "mint" --args $BTC 1000000000`

### Mint ETH
`sui client call --gas-budget 10000 --package $TOKEN_PACKAGE --module "eth" --function "mint" --args $ETH 1000000000`

### Mint SUI
`sui client call --gas-budget 10000 --package $TOKEN_PACKAGE --module "sui" --function "mint" --args $SUI 1000000000`

### Mint USDC
`sui client call --gas-budget 10000 --package $TOKEN_PACKAGE --module "usdc" --function "mint" --args $USDC 1000000000`

