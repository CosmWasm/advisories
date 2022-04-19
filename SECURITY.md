# Security Policy

This is a shared security policy for the CosmWasm stack, including the following repositories:

- [cosmwasm](https://github.com/CosmWasm/cosmwasm)
- [wasmvm](https://github.com/CosmWasm/wasmvm)
- [wasmd](https://github.com/CosmWasm/wasmd)
- [cw-plus](https://github.com/CosmWasm/cw-plus)
- [rust-optimizer](https://github.com/CosmWasm/rust-optimizer)
- [serde-json-wasm](https://github.com/CosmWasm/serde-json-wasm)

## Reporting a Vulnerability

Please report any security issues via email to security@confio.gmbh.

You will receive a response from us within 2 working days. If the issue is confirmed, we will release a patch as soon as possible depending on complexity but historically within a few days.

Please avoid opening public issues on GitHub that contain information about a potential security vulnerability as this makes it difficult to reduce the impact and harm of valid security issues.

## Supported Versions

The supported versions are described in more detail in the individual repositories. This is a summary:

- [CosmWasm](https://github.com/CosmWasm/cosmwasm): 1.x
- [wasmvm](https://github.com/CosmWasm/wasmvm): 1.x
- [wasmd](https://github.com/CosmWasm/wasmd): 1.x

## Coordinated Vulnerability Disclosure Policy

We ask security researchers to keep vulnerabilities and communications around vulnerability submissions private and confidential until a patch is developed. In addition to this, we ask that you:

- Allow us a reasonable amount of time to correct or address security vulnerabilities.
- Avoid exploiting any vulnerabilities that you discover.
- Demonstrate good faith by not disrupting or degrading services built on top of this software.

## Vulnerability Disclosure Process

Confio uses the following disclosure process for the various CosmWasm-related repos:

- Once a security report is received, the core development team works to verify the issue.
- Patches are prepared for eligible releases in private repositories.
- We notify the community that a security release is coming, to give users time to prepare their systems for the update.
  - The notification contains the release date and time (72-24 hours after the notification).
  - The notification contains as little information as possible to make it hard for attackers to guess where to search. However, depending on the situation it may contain additional information such as whether or not the patch will be consensus breaking or chains with permissioned CosmWasm integration are equally affected as permissionless chains.
  - The projects on the [notification list](https://github.com/CosmWasm/advisories#notification-list) is informed first. Please add yourself via a PR if you want to receive notifications.
  - Right after that the notification is broadcasted publically including Discord messages, tweets, and emails to partners and validators.
- The fixes are applied publicly and new releases are issued.
- Once releases are available, we notify the community, again, through the same channels as above.
- Once the patches have been properly rolled out and no earlier than 7 days after the release, we will publish a post with further details on the vulnerability as well as our response to it.
- Note that we are working on a concept for bug bounties and they are not currently available.

This process can take some time. Every effort will be made to handle the bug as quickly and thoroughly as possible. However, it's important that we follow the process described above to ensure that disclosures are handled consistently and to keep this codebase and the projects that depend on them secure.
