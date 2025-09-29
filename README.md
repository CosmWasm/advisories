[cosmwasm]: https://github.com/CosmWasm/cosmwasm
[wasmvm]: https://github.com/CosmWasm/wasmvm
[wasmd]: https://github.com/CosmWasm/wasmd

# CosmWasm Advisories

We work in the best intent with a public review process but must accept
that software can contain bugs and therefore CosmWasm code, too.

In order to help with resolving any issues on production system, we are maintaining
the advisories project to link to authorized communication channels of CosmWasm blockchains.
Linked chains will be informed about **critical issues** reported to us directly
on **non-public channels** before opening an issue on our related projects.
Nevertheless, providing this information should not prevent anyone from working
on a fix nor block a patch roll out. This also does not include bugs and issues reported
to us publicly via GitHub issues or other official channels. Chains using our projects
are encouraged to **watch the GitHub repositories and official channels** in order
to maintain their own software stack.

## Supported projects and version

- CosmWasm ([cosmwasm-\*][cosmwasm] and [wasmvm])
  - ~1.2.x ([until 2023-12-31](https://medium.com/cosmwasm/eol-for-cosmwasm-1-0-1-3-22df4b34b13c))~
  - ~1.3.x ([until 2024-03-31](https://medium.com/cosmwasm/eol-for-cosmwasm-1-0-1-3-22df4b34b13c))~
  - ~1.4.x ([until 2024-07-31](https://medium.com/cosmwasm/cosmwasm-1-5-becomes-long-term-support-lts-version-16632bf06f2a))~
  - ~1.5.x ([until 2025-04-30](https://medium.com/cosmwasm/cosmwasm-2-2-becomes-long-term-support-lts-version-7fdd6a507485))~
  - ~2.0.x ([until 2025-01-31](https://medium.com/cosmwasm/cosmwasm-2-2-becomes-long-term-support-lts-version-7fdd6a507485))~
  - ~2.1.x ([until 2025-01-31](https://medium.com/cosmwasm/cosmwasm-2-2-becomes-long-term-support-lts-version-7fdd6a507485))~
  - 2.2.x ([until 2025-12-31](https://medium.com/cosmwasm/cosmwasm-2-2-becomes-long-term-support-lts-version-7fdd6a507485))
- [wasmd]
  - 1.0.x

## Criteria to get on the notification list

- Running CosmWasm projects **on production** or public testnet.
- `SECURITY.md` file placed in your main repo and main branch with contact details and infos on your disclosure process.
- Commitment to share issues and bugs with CosmWasm community.

If your project meets these criteria, please submit a PR to add your chain to the [list below](#notification-list).

## Disclaimer

We likely will not have capacity to maintain this service for all versions and projects forever.

So we want to keep the right to:

- modify this document,
- add/remove project and versions,
- change the criteria and revisit the listed members,
- not accept every application.

## Notification list

See [NOTIFICATION_LIST.md](NOTIFICATION_LIST.md)
