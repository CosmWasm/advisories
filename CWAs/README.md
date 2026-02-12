# Index of CosmWasm Advisories

## 2025

| [Severity] | [Scope] | ID                                                                                                  | Aliases               |
|------------|---------|-----------------------------------------------------------------------------------------------------|-----------------------|
| Medium     | x/wasm  | [CWA-2025-007: Unbounded reply recursion causing stack overflow][CWA-2025-007]                      |                       |
| High       | x/wasm  | [CWA-2025-006: Improper error handling may lead to IBC channel opening despite error][CWA-2025-006] |                       |
| Medium     | x/wasm  | [CWA-2025-005: Missing contract setup cost for IBC entrypoints][CWA-2025-005]                       |                       |
| Low        | x/wasm  | [CWA-2025-004: Sub-context gas not consumed on non-OutOfGas panics][CWA-2025-004]                   |                       |
| Low        | VM      | [CWA-2025-003: Smart contract can cause consensus failures for some nodes][CWA-2025-003]            |                       |
| Medium     | VM      | [CWA-2025-002: Malicious smart contract can slow down block production][CWA-2025-002]               | [GHSA-mx2j-7cmv-353c] |
| Medium     | VM      | [CWA-2025-001: Malicious smart contract can crash the chain][CWA-2025-001]                          | [GHSA-23qp-3c2m-xx6w] |

[CWA-2025-007]: ./CWA-2025-007.md
[CWA-2025-006]: ./CWA-2025-006.md
[CWA-2025-005]: ./CWA-2025-005.md
[CWA-2025-004]: ./CWA-2025-004.md
[CWA-2025-003]: ./CWA-2025-003.md
[CWA-2025-002]: ./CWA-2025-002.md
[CWA-2025-001]: ./CWA-2025-001.md
[GHSA-mx2j-7cmv-353c]: https://github.com/CosmWasm/wasmvm/security/advisories/GHSA-mx2j-7cmv-353c
[GHSA-23qp-3c2m-xx6w]: https://github.com/CosmWasm/wasmvm/security/advisories/GHSA-23qp-3c2m-xx6w

## 2024

| [Severity] | [Scope]   | ID                                                                           | Aliases                                    |
|------------|-----------|------------------------------------------------------------------------------|--------------------------------------------|
| Low        | VM        | [CWA-2024-009][CWA-2024-009]                                                 | [GHSA-vmg2-r3xv-r3xf]                      |
| Medium     | VM        | [CWA-2024-008: Panic in wasmvm can slow down block production][CWA-2024-008] | [GHSA-vmqh-5232-v43r]                      |
| Medium     | VM        | [CWA-2024-007: Incorrect metering][CWA-2024-007]                             | [GHSA-2q97-m5rc-p3gp]                      |
| Medium     | x/wasm    | [CWA-2024-006: Non-deterministic module_query_safe query][CWA-2024-006]      | [GHSA-fpgj-cr28-fvpx]                      |
| High       | x/wasm    | [CWA-2024-005: Stackoverflow in wasmd][CWA-2024-005]                         | [GHSA-g8w7-7vgg-x7xg]                      |
| Medium     | VM        | [CWA-2024-004: Gas mispricing in cosmwasm-vm][CWA-2024-004]                  | [RUSTSEC-2024-0361], [GHSA-rg2q-2jh9-447q] |
| Low        | x/wasm    | [CWA-2024-003: Large address count in ValidateBasic][CWA-2024-003]           | [GHSA-m3rh-cvr5-x6q4]                      |
| Medium     | Contracts | [CWA-2024-002: Arithmetic overflows in cosmwasm-std][CWA-2024-002]           | [RUSTSEC-2024-0338], [GHSA-8724-5xmm-w5xq] |
| Low        | Contracts | [CWA-2024-001: Stack overflow in serde-json-wasm][CWA-2024-001]              | [RUSTSEC-2024-0012], [GHSA-rr69-rxr6-8qwf] |

[CWA-2024-009]: ./CWA-2024-009.md
[CWA-2024-008]: ./CWA-2024-008.md
[CWA-2024-007]: ./CWA-2024-007.md
[CWA-2024-006]: ./CWA-2024-006.md
[CWA-2024-005]: ./CWA-2024-005.md
[CWA-2024-004]: ./CWA-2024-004.md
[CWA-2024-003]: ./CWA-2024-003.md
[CWA-2024-002]: ./CWA-2024-002.md
[CWA-2024-001]: ./CWA-2024-001.md
[RUSTSEC-2024-0338]: https://rustsec.org/advisories/RUSTSEC-2024-0338.html
[RUSTSEC-2024-0012]: https://rustsec.org/advisories/RUSTSEC-2024-0012.html
[RUSTSEC-2024-0361]: https://rustsec.org/advisories/RUSTSEC-2024-0361.html
[GHSA-8724-5xmm-w5xq]: https://github.com/advisories/GHSA-8724-5xmm-w5xq
[GHSA-rr69-rxr6-8qwf]: https://github.com/advisories/GHSA-rr69-rxr6-8qwf
[GHSA-rg2q-2jh9-447q]: https://github.com/advisories/GHSA-rg2q-2jh9-447q
[GHSA-m3rh-cvr5-x6q4]: https://github.com/advisories/GHSA-m3rh-cvr5-x6q4
[GHSA-g8w7-7vgg-x7xg]: https://github.com/advisories/GHSA-g8w7-7vgg-x7xg
[GHSA-fpgj-cr28-fvpx]: https://github.com/advisories/GHSA-fpgj-cr28-fvpx
[GHSA-2q97-m5rc-p3gp]: https://github.com/CosmWasm/wasmvm/security/advisories/GHSA-2q97-m5rc-p3gp
[GHSA-vmqh-5232-v43r]: https://github.com/CosmWasm/wasmvm/security/advisories/GHSA-vmqh-5232-v43r
[GHSA-vmg2-r3xv-r3xf]: https://github.com/CosmWasm/wasmd/security/advisories/GHSA-vmg2-r3xv-r3xf

## 2023

| [Severity] | [Scope] | ID                                                                                    |
|------------|---------|---------------------------------------------------------------------------------------|
| High       | VM      | [CWA-2023-004: Excessive number of function paramters in compiled Wasm][CWA-2023-004] |
| Medium     | x/wasm  | [CWA-2023-003: Inefficient ListChannels query implementation][CWA-2023-003]           |
|            | VM      | [CWA-2023-002: Stack overflow crash (Codename Cherry)][CWA-2023-002]                  |
|            | VM      | [CWA-2023-001: Potential overflow in cache statistics][CWA-2023-001]                  |

[CWA-2023-004]: ./CWA-2023-004.md
[CWA-2023-003]: ./CWA-2023-003.md
[CWA-2023-002]: ./CWA-2023-002.md
[CWA-2023-001]: ./CWA-2023-001.md

## 2022

| [Severity] | [Scope] | ID                                                                                     |
|------------|---------|----------------------------------------------------------------------------------------|
|            | x/wasm  | [CWA-2022-005: Denial of service through predictable contract addresses][CWA-2022-005] |
|            | x/wasm  | [CWA-2022-004: Unlimited query stack][CWA-2022-004]                                    |
|            | x/wasm  | [CWA-2022-003: Nondeterministic Stargate queries][CWA-2022-003]                        |
|            | VM      | [CWA-2022-002: Non-normalized bech32 casing in Addr type][CWA-2022-002]                |
|            | x/wasm  | [CWA-2022-001: Non-deterministic queries][CWA-2022-001]                                |

[CWA-2022-005]: ./CWA-2022-005.md
[CWA-2022-004]: ./CWA-2022-004.md
[CWA-2022-003]: ./CWA-2022-003.md
[CWA-2022-002]: ./CWA-2022-002.md
[CWA-2022-001]: ./CWA-2022-001.md

## 2021

| [Severity] | [Scope] | ID                                                                                          |
|------------|---------|---------------------------------------------------------------------------------------------|
|            | VM      | [CWA-2021-003: Nondeterministic stacktrace in VmError][CWA-2021-003]                        |
|            |         | CWA-2021-002: reserved                                                                      |
|            | VM      | [CWA-2021-001: Logic error in none handling in copyAndDestroyUnmanagedVector][CWA-2021-001] |

[CWA-2021-003]: ./CWA-2021-003.md
[CWA-2021-002]: ./CWA-2021-002.md
[CWA-2021-001]: ./CWA-2021-001.md


[Severity]: #Severity
[Scope]: #Scope

---

### Severity

Following Amulet's Severity Classification Framework ACMv1: https://github.com/interchainio/security/blob/e0227a1fb4059144aab4f6003eeee7f09912db3a/resources/CLASSIFICATION_MATRIX.md

### Scope

- **Contracts** - everything compiled into Wasm (cosmwasm-std, other contract libraries),
- **VM** - everything executing contracts (cosmwasm-vm, wasmvm), 
- **x/wasm** - integration of the VM into the chain (wasmd).
