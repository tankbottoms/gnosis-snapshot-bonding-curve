# snapshot examples

The snapshot files within this directory include

- addresses,
- contributions,
- block number,
- timestamp,
- other metadata,
  for which is used to compute various token distributions

The `.csv` file contains addresses and amounts of contributions.

```typescript
const FREEROSSDAO = {
  name: 'free-ross-dao',
  address: '0xc102d2544a7029f7BA04BeB133dEADaA57fDF6b4',
  deployed_block: 13_724_221,
  auction_end_block: 13_770_208,
};
```

Capturing the snapshot of a gnosis safe is handled by the following tool:

```sh
npx ts-node ./scripts/snapshot.ts
```

## bonding curve

1. endowment-seeders.ts
2. [freerossdao-contributors.csv]\* - this file is used with endowment-seeders.ts to compute the bonding curve pricing

- For development purposes, the freerossdao addresses and purchase amounts are used in place of the move.eth token contributions.

## developer communities

1. `openlaw-dao-members.ts`
2. `openlaw-dao-developers.ts`
3. `juicebox-community.ts`

## community airdrops

1. `dao-participants.ts`
2. `ens.ts`
3. `opensea.ts`

### methods

- in order to extract community members who have interacted with JBX access the transactions history of those that interacted with the JBX terminal contract, Tap method for distributing payout to contributors and Pay/Redeem method for buy/sell with projects on JBX platform...
