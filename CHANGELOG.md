# CHANGELOG

## v0.8.0

*Apr 26, 2023*

This release bumps the supported version of RocksDB, which requires cometbft-db
RocksDB users to update their builds (and hence requires a "major" release, but
does not introduce any other breaking changes). Special thanks to @yihuang for
this update!

While the minimum supported version of the Go compiler was bumped to 1.19, no
1.19-specific code changes were introduced and this should, therefore, still be
able to be compiled with earlier versions of Go. It is, however, recommended to
upgrade to the latest version(s) of Go ASAP.

### COMPILER

- Bump minimum Go version to 1.19
  ([\#40](https://github.com/opzlabs/cometbft-db/pull/40))

### DEPENDENCIES

- Update to the latest version of golang.org/x/net
  ([\#40](https://github.com/opzlabs/cometbft-db/pull/40))
- Switch rocksdb binding from gorocksdb to grocksdb, bump librocksdb dependency
  to `v7.10.2` ([\#42](https://github.com/opzlabs/cometbft-db/pull/42))

## v0.7.0

*Jan 17, 2023*

This is the first official release of CometBFT DB, which is a fork of
[tm-db](https://github.com/tendermint/tm-db).

This fork is intended to be used by
[CometBFT](https://github.com/cometbft/cometbft) until such time that
[cometbft/cometbft\#48](https://github.com/cometbft/cometbft/issues/48) is
resolved, after which time this fork will be retired and archived. Do not use
this as a dependency in any new projects.

### BREAKING CHANGES

- Fork tm-db and rename fork to cometbft-db
  ([\#7](https://github.com/opzlabs/cometbft-db/issues/7))

---

CometBFT DB is a fork of [tm-db](https://github.com/tendermint/tm-db)
effectively as of v0.6.6.

For changes prior to the creation of this fork, please refer to the upstream
[CHANGELOG.md](https://github.com/tendermint/tm-db/blob/774cdfe7e6b0a249b1144998d81a4de7b8037941/CHANGELOG.md)
for v0.6.6 and earlier.

