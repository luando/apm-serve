# apm-serve
Web 2.0 server for Web 3.0 APM hosted dApps

## Goal API

- `dapp.aragonpm.com` -> serves content from latest version of dapp.aragonpm.eth in the mainnet
- `dapp.rinkeby.aragonpm.com` -> serves content from latest version of dapp.aragonpm.eth in rinkeby (requires setting ENS address)
- `1.2.3.dapp.aragonpm.com` -> serves version 1.2.3 of dapp
- `voting.aragonpm.com/?json=true` -> serves json with all versions of voting.aragonpm.eth with smart contract addresses and contentURIs
- `voting.aragonpm.com/?json=true&version=1.2.3` -> serves version information for voting.aragonpm.eth 1.2.3

## What about running it on myregistry.eth?

- Use the docker image to deploy to your hosting service of choice and configure it for your registry

## Roadmap

- v1: HTTP serve contentURI of a given package, for different networks and versions.
- v2: JSON API
- v3: DNS gateway like ipfs-gateway, that would allow just running 1 instance of `apm-serve`
and people being able to serve registries or specific content just by configuring DNS.
