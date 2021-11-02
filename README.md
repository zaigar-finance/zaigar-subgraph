# Zaigar Finance Subgraph

TheGraph exposes a GraphQL endpoint to query the events and entities within the Binance Smart Chain.

Currently, there are zai Option subgraph, but additional subgraphs can be added to this repo:


1. **[ZaiOption](https://thegraph.com/hosted-service/subgraph/zaigar-finance/zai-option-v1)**: Tracks all Zaigar Finance zaiOption with market, rounds, and bets.


## To setup and deploy

For any of the subgraph: `blocks` as `[subgraph]`

1. Run the `cd subgraphs/[subgraph]` command to move to the subgraph directory.

2. Run the `yarn codegen` command to prepare the TypeScript sources for the GraphQL (generated/*).

3. Run the `yarn build` command to build the subgraph, and check compilation errors before deploying.

4. Run `graph auth --product hosted-service '<ACCESS_TOKEN>'`

5. Deploy via `yarn deploy`.
