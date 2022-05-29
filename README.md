# subgraph-wbtc
#Step for create project
- Create a Subgraph https://thegraph.com/studio/
- graph init --studio subgraph-wbtc
- graph auth --studio <api_key>
- cd subgraph-wbtc
- graph codegen && graph build
- graph deploy --studio subgraph-wbtc

#Query subgraph
- {
  transferEntities(first: 100) {
    txHash
    id
    from
    to
    value
  }
}
