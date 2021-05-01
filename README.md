# Ethereum Sentry Fork
Service that listens to Ethereum's P2P network, serves information to other nodes, and provides gRPC interface to clients to interact with the network.

# Running
`env RUST_LOG=ethereum_sentry cargo run --release`

# Options
Run `cargo run --release -- --help` to see the full list of options.

# Run
```
cargo build
./target/debug/ethereum-sentry
```
Should see something like:
```
May 01 16:52:36.004  INFO ethereum_sentry: Generated new node key: 88a53f8360fc908c7d40a65b90ac3bace963ddc6f04993e639ddf4e196c52438
May 01 16:52:36.005  INFO ethereum_sentry: Starting Ethereum sentry
May 01 16:52:36.027  INFO ethereum_sentry: Node ID: e18c29b11f62d35cdd021e1ff1fbe7db35319153323f5f3f34cb9bc7154a9423eac39552dfc1c1e9539f1cb52bb8ab99e96ff20febb1c2f56d6c381ad017d49c
May 01 16:52:36.027  INFO ethereum_sentry: Starting DNS discovery fetch from all.mainnet.ethdisco.net
May 01 16:52:36.029  INFO ethereum_sentry: Starting discv4 at port 30303
May 01 16:52:36.031  INFO ethereum_sentry: Using default discv4 bootstrap nodes
May 01 16:52:36.034  INFO ethereum_sentry: RLPx node listening at 0.0.0.0:30303
May 01 16:52:36.034  INFO ethereum_sentry: Peer info: 0 active (+0 dialing) / 50 max.
May 01 16:52:36.035  INFO ethereum_sentry: Sentry gRPC server starting on 0.0.0.0:8000
May 01 16:52:41.040  INFO ethereum_sentry: Peer info: 0 active (+0 dialing) / 50 max.
May 01 16:52:43.766  WARN discv4::node: Failed to handle message from 3.36.125.131:30303: Hash check failed: computed 0xa510…ac82, prefix 0x9a90…e55a
May 01 16:52:46.042  INFO ethereum_sentry: Peer info: 0 active (+0 dialing) / 50 max.
May 01 16:52:51.047  INFO ethereum_sentry: Peer info: 0 active (+0 dialing) / 50 max.
May 01 16:52:56.050  INFO ethereum_sentry: Peer info: 0 active (+0 dialing) / 50 max.
May 01 16:53:01.057  INFO ethereum_sentry: Peer info: 0 active (+0 dialing) / 50 max.
May 01 16:53:06.063  INFO ethereum_sentry: Peer info: 0 active (+0 dialing) / 50 max.
```
