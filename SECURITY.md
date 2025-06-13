# Security Policy

This is a shared security policy for the CosmWasm stack, including the following repositories:

- Execution environment
  - [cosmwasm]
  - [wasmvm]
  - [wasmd]
- Standard library dependencies
  - [serde-json-wasm]
- Libraries for building contracts
  - [cw-plus]
  - [cw-storage-plus]
  - [cw-utils]
- Build tools
  - [rust-optimizer]

## Reporting a Vulnerability

There are three ways to report a security issue

|                     | Cosmos HackerOne Bug Bounty program                   | security<span>@</span>interchain.io                                                                                                                                                                                                                                                                 | security<span>@</span>confio.gmbh                                                                                                                                                                                                 |
| ------------------- | ----------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Maintained by       | Interchain Labs                                       | Interchain Labs                                                                                                                                                                                                                                                                                     | Confio                                                                                                                                                                                                                            |
| Eligible for bounty | yes                                                   | no                                                                                                                                                                                                                                                                                                  | no                                                                                                                                                                                                                                |
| Reporting link      | <https://hackerone.com/cosmos>                        | [security@interchain.io](mailto:security@interchain.io)                                                                                                                                                                                                                                             | [security@confio.gmbh](mailto:security@confio.gmbh)                                                                                                                                                                               |
| Reporter management | professional communication                            | professional communication                                                                                                                                                                                                                                                                          | best effort                                                                                                                                                                                                                       |
| Details             | See program details at <https://hackerone.com/cosmos> | If you prefer to report an issue via email, you may send a bug report to security@interchain.io with the issue details, reproduction, impact, and other information. Please submit only one unique email thread per vulnerability. Any issues reported via email are ineligible for bounty rewards. | You will receive a response from us within 4 working days confirming that a human read your email. If you do not hear back within 1 week, feel free to send a reminder or try to notify core team members via different channels. |

Please only choose one. In all cases the analysis and fixing of the issue will be performed by Confio.

Within a few days we try to reproduce the issue and confirm it. After that we work on a patch and a release strategy. Experience shows the later part is harder than the actual patch as we need to evaluate which versions are affected, for which versions a patch is provided, if that patch is consensus or state breaking and how users can apply the patch. This part can take a few days up to multiple weeks.

Please avoid opening public issues on GitHub that contains information about a potential security vulnerability as this makes it difficult to reduce the impact and harm of valid security issues.

## Supported Versions

The supported versions are described in more detail in the individual repositories. This is a summary:

- CosmWasm ([cosmwasm-\*][cosmwasm] and [wasmvm])
  - 1.2.x ([until 2023-12-31](https://medium.com/cosmwasm/eol-for-cosmwasm-1-0-1-3-22df4b34b13c))
  - 1.3.x ([until 2024-03-31](https://medium.com/cosmwasm/eol-for-cosmwasm-1-0-1-3-22df4b34b13c))
  - 1.4.x
  - 1.5.x
  - 2.0.x
- [wasmd] 1.x
- [cw-plus], [cw-storage-plus], [cw-utils] 1.x

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
  - The notification contains as little information as possible, to make it hard for attackers to guess where to search. However, depending on the situation it may contain additional information such as whether the patch will be consensus breaking, or if chains with permissioned CosmWasm integration are equally affected as permissionless chains.
  - The projects on the [notification list](https://github.com/CosmWasm/advisories#notification-list) are informed first. Please add yourself via a PR if you want to receive notifications.
  - Right after that the notification is publicly broadcast, including Discord messages, tweets, and emails to partners and validators.
- The fixes are applied publicly and new releases are issued.
- Once releases are available, we notify the community, again, through the same channels as above.
- Once the patches have been properly rolled out and no earlier than 7 days after the release, we will publish a post with further details on the vulnerability as well as our response to it.
- Note that we are working on a concept for bug bounties and they are not currently available.

This process can take some time. Every effort will be made to handle the bug as quickly and thoroughly as possible. However, it's important that we follow the process described above to ensure that disclosures are handled consistently and to keep this codebase and the projects that depend on them secure.

### Exceptions

Please note that issues are considered already disclosed if there is a public patch for it or it is discussed in public (e.g. CWA-2023-001). In those cases the above process does not apply.
An exception can be cases where the fix was well hidden and neither the fix not the public discussion reveals
a vulnerability was patched (e.g. CWA-2022-005).
Advisories are created and published in any case for future reference, giving credit to the people involved and the learning opportunity.

[cosmwasm]: https://github.com/CosmWasm/cosmwasm
[cw-plus]: https://github.com/CosmWasm/cw-plus
[cw-storage-plus]: https://github.com/CosmWasm/cw-storage-plus
[cw-utils]: https://github.com/CosmWasm/cw-utils
[serde-json-wasm]: https://github.com/CosmWasm/serde-json-wasm
[rust-optimizer]: https://github.com/CosmWasm/rust-optimizer
[wasmd]: https://github.com/CosmWasm/wasmd
[wasmvm]: https://github.com/CosmWasm/wasmvm
