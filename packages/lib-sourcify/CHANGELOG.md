# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## [2.0.1](https://github.com/ethereum/sourcify/compare/@ethereum-sourcify/lib-sourcify@2.0.0...@ethereum-sourcify/lib-sourcify@2.0.1) (2025-04-25)

### Bug Fixes

- **deps:** update all patch and minor dependencies ([d439283](https://github.com/ethereum/sourcify/commit/d439283e16b00c4f8ef196c7ae3a4ae889061c33))
- **deps:** update all patch and minor dependencies ([#2096](https://github.com/ethereum/sourcify/issues/2096)) ([49af4a6](https://github.com/ethereum/sourcify/commit/49af4a64bb0a72b6224927d732485ff9a337031d))

## @ethereum-sourcify/lib-sourcify@2.0.0 - 2025-04-09

- (Breaking change) Complete refactoring of the verification flow (#1845)
- Add Validation classes and types (#1851)
- Add Compilation classes and types (#1849)
- Implement tests for the new verification flow
- Implement SolidityMetadataContract (#1869)
- Add Verification classes (#1879)
- Improve auxdata position generation return types and error handling (#1993)
- Add VerificationExport (#1994)

## @ethereum-sourcify/lib-sourcify@1.13.0 - 2025-03-19

- Use @ethereum-sourcify/compilers package instead of built-in compiler
- Update dependencies

## @ethereum-sourcify/lib-sourcify@1.12.1 - 2025-02-18

- update dependencies

## @ethereum-sourcify/lib-sourcify@1.12.0 - 2025-02-06

- Fix perfect creation matching when CBOR is not at the end

## @ethereum-sourcify/lib-sourcify@1.11.0 - 2025-01-08

- Add Vyper verification support
- Update dependencies

## @ethereum-sourcify/lib-sourcify@1.10.1 - 2024-12-11

- Add SourcifyChain.getStorageAt
- Update dependencies

## @ethereum-sourcify/lib-sourcify@1.10.0 - 2024-10-29

- Add RPCs with trace support in SourcifyChains
- Add support for getting the tx traces from `trace_transaction` and `debug_traceTransaction` type traces.
- Update packages

## @ethereum-sourcify/lib-sourcify@1.9.3 - 2024-10-14

- Add routescan for creatorTx fetching and types
- Update packages

## @ethereum-sourcify/lib-sourcify@1.9.2 - 2024-09-17

- Fix wrong bytecode comparison on creation bytecode matching, use .startsWith() instead
- Fix the check for already existing partial match
- Added test for above cases

## @ethereum-sourcify/lib-sourcify@1.9.1 - 2024-08-29

- Add custom headers for the IPFS Gateway
- Fix passing the runtimeMatch when matching with the creation bytecode
- Add logs
- Update packages

## @ethereum-sourcify/lib-sourcify@1.9.0 - 2024-07-25

- Update dependencies
- Fix saving the user input metadata.json instead of the compiler's output metadata.json
- Use linkReferences to find and parse linked libraries in the bytecode instead of the placeholder. Also save fully qualified lib names in the transformations instead of placeholders.
- Change Transformation names to be consistent with Transformations and TransormationValues

## @ethereum-sourcify/lib-sourcify@1.8.0 - 2024-05-14

- Support for verification with double metadata hash (auxdata)
- Added test for multiple auxdata
- Change error logs to info level

## @ethereum-sourcify/lib-sourcify@1.7.5 - 2024-04-23

- Add log to fetching bytecode

## @ethereum-sourcify/lib-sourcify@1.7.4 - 2023-04-04

- Add function to export the minimum information to reconstruct the CheckedContract

## @ethereum-sourcify/lib-sourcify@1.7.3 - 2023-03-28

- Update logging

## @ethereum-sourcify/lib-sourcify@1.7.2 - 2023-03-14

- Fix bytecode transformations

## @ethereum-sourcify/lib-sourcify@1.7.1 - 2023-02-26

- Fix `fsevents` to the `optionalDependencies` for Linux builds.

## @ethereum-sourcify/lib-sourcify@1.7.0 - 2023-02-22

- Support verification for bytecode containing multiple auxdatas.
  - Use `generateCborAuxdataPositions` to locate the auxdata positions in the bytecode and ignore them for a partial match.
- Add `blockNumber`, `txIndex`, and `deployer` to the `Match` type

## @ethereum-sourcify/lib-sourcify@1.6.2 - 2023-01-03

- Don't fetch `creationTx` twice
- More detailed debug logging.

## @ethereum-sourcify/lib-sourcify@1.6.1 - 2023-12-19

- Bump Typscript version and move the dependency to project root.
- Change SourcifyChainExtension types, according to the new sourcify-server's `sourcify-chains.json` format.

## @ethereum-sourcify/lib-sourcify@1.6.0 - 2023-11-23

- Remove solc as a dependency, now it must be included implementing the `ISolidityCompiler` interface
- fix `extra-file-input-bug`

## @ethereum-sourcify/lib-sourcify@1.5.0 - 2023-11-03

- Remove solc as a dependency, now the solidity compiler needs to be passed to the functions using it.
- Rename deployedBytecode into runtimeBytecode
- Use `fetchContractCreationTxUsing` object to scrape
- Always comoapile with emscripten for nightlies and versions <0.4.10
- Support creationMatch vs runtimeMatch

## @ethereum-sourcify/lib-sourcify@1.4.2 - 2023-10-19

- Bump to sync the tags on master

## @ethereum-sourcify/lib-sourcify@1.4.1 - 2023-10-18

- Remove `typeRoots` from `tsconfig.json`

## @ethereum-sourcify/lib-sourcify@1.4.0 - 2023-10-09

- Bump `ethers` to `6.7.1`
- Bump `solc` to `0.8.21`
- Split `MetadataSources` type to `MetadataSourceMap` and `MetadataSource`
- Remove package-lock.json as it is managed by root package.json by lerna

## @ethereum-sourcify/lib-sourcify@1.3.2 - 2023-09-04

- Use `https://binaries.soliditylang.org` instead of `https://github.com/ethereum/solc-bin/raw/gh-pages` for Solidity compiler binaries

## Older releases

Previously, the releases were not done one separate modules of Sourcify but for the repository as a whole.
You can find the changelog for those releases in [older releases](https://github.com/ethereum/sourcify/releases) for this repository.
