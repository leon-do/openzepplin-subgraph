# OpenZeppelin Subgraph

Deploys [Open Zepplin Subgraphs](https://docs.openzeppelin.com/subgraphs/0.1.x/) to Subgraph Studio

## The Graph Deployment

[Create a Subgraph](https://thegraph.com/studio/)

Create a file in `config/` named after the network you want to deploy to, e.g. `config/celo.json`

```json
{
  "output": "generated/celo",
  "chain": "celo",
  "datasources": [
    {
      "startBlock": 0,
      "module": ["erc20", "erc721", "erc1155"]
    }
  ]
}
```

In `package.json` add a script for the network you want to deploy to, e.g.

```json
{
  "celo": "graph-compiler --config config/celo.json --include node_modules/@openzeppelin/subgraphs/src/datasources --export-schema --export-subgraph && graph codegen generated/celosubgraph.yaml && graph build generated/celosubgraph.yaml && graph deploy --studio celo-tokens generated/celosubgraph.yaml",
}
```

## Networks

| Network    | Link |
| -------- | ------- |
|`arbitrum-nova` | [Subgraph](https://thegraph.com/explorer/subgraphs/GwV8GCTtXrFYkMeXWMnCGKcXCj5Ybm5aWEb8KmHWNYVE) |
| `arbitrum-one` | [Subgraph](https://thegraph.com/explorer/subgraphs/Uzw5rTCvFYiHeNgzioHo5GSge4WqPMQdbk6xQLRHE5C?view=Query&chain=arbitrum-one) |
| `astar-zkevm-mainnet` | Subgraph |
| `aurora` | [Subgraph](https://thegraph.com/explorer/subgraphs/2tbJ9TKWm3nfxrSFYxS6wdTdpARsWWmjNjcpAoGMB9Eu?view=Query&chain=arbitrum-one) |
| `avalanche` | [Subgraph](https://thegraph.com/explorer/subgraphs/6gdhDA1hu5RcDikVYBN8JMvX6mfWsa5ooMB6KWdTXNF8?view=Query&chain=arbitrum-one) |
| `base` | [Subgraph](https://thegraph.com/explorer/subgraphs/FdHA7Y1AMvMTjrMjuguyRmf9CcQD26GUdjCKrijdq8wj?view=Query&chain=arbitrum-one) |
| `blast-mainnet` | [Subgraph](https://thegraph.com/explorer/subgraphs/6UzrsoSrqaYubtGmHcrW7upQ4AucLeSZhYCsRZURozu2?view=Query&chain=arbitrum-one) |
| `boba` | [Subgraph](https://thegraph.com/explorer/subgraphs/9PDtS6gk2z7EQKiQtvUTX3C9PViUpd4DfpAQvhyF93gU?view=Query&chain=arbitrum-one) |
| `bsc` | Subgraph |
| `celo` | [Subgraph](https://thegraph.com/explorer/subgraphs/FPEBHRgUBTzUeqf8CsX9nCPXU9zjdPhGrye7Q41qc5vA?view=Query&chain=arbitrum-one) |
| `etherlink-mainnet` | Subgraph |
| `fantom` | Subgraph |
| `fuse` | Subgraph |
| `gnosis` | Subgraph |
| `gravity-mainnet` | [Subgraph](https://thegraph.com/explorer/subgraphs/4fzjXbSJpxK2awqEotMY4NWZJCosuYRyafV19k5fss57?view=Query&chain=arbitrum-one) |
| `harmony` | [Subgraph](https://thegraph.com/explorer/subgraphs/TaYQ4vW1Ljs3whxYYegdg8DqAXGwsD5xQjiZqkiLPZF?view=Query&chain=arbitrum-one) |
| `iotex` | Subgraph |
| `linea` | Subgraph |
| `mainnet` | [Subgraph](https://thegraph.com/explorer/subgraphs/ATgNVs4BDe3UiRinMWxPu49bntsKBPSip9ejVZJ2GRVt?view=Query&chain=arbitrum-one) |
| `matic` | Subgraph |
| `mode-mainnet` | Subgraph |
| `moonbeam` | Subgraph |
| `moonriver` | Subgraph |
| `neox` | Subgraph |
| `optimism` | Subgraph |
| `polygon-zkevm` | Subgraph |
| `rootstock` | Subgraph |
| `scroll` | Subgraph |
| `sei-mainnet` | Subgraph |
| `xlayer-mainnet` | Subgraph |
| `zksync-era` | Subgraph | 


