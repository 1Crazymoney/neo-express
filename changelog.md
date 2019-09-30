# NEO Express Change Log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

This project uses [NerdBank.GitVersioning](https://github.com/AArnott/Nerdbank.GitVersioning)
to manage version numbers. This tool automatically sets the Semantic Versioning Patch
value based on the [Git height](https://github.com/AArnott/Nerdbank.GitVersioning#what-is-git-height)
of the commit that generated the build. As such, released versions of this extension
will not have contiguous patch numbers. Initial major and minor releases will be documented
in this file without a patch number. Patch version will be included for bug fix releases, but
may not exactly match a publicly released version.

## [0.9] - Unreleased

- Refactored neo-express to merge abstraction and express2 libraries back into
  neo-express. This separation was originally done to enable neo-express to support
  NEO 2 and 3, however this approach would not work, so it was undone.
- Exposed Debug port, compatible with Microsoft's
  [Debug Adapter Protocol](https://microsoft.github.io/debug-adapter-protocol/specification)
  and the [NEO Smart Contract Debugger for VSCode](https://github.com/neo-project/neo-debugger).
- added [getunspents](https://docs.neo.org/docs/en-us/reference/rpc/latest-version/api/getunspents.html),
  [getunclaimed](https://docs.neo.org/docs/en-us/reference/rpc/latest-version/api/getunclaimed.html)
  and [getunclaimedgas](https://docs.neo.org/docs/en-us/reference/rpc/latest-version/api/getunclaimedgas.html)
  RPC endpoints.
- added support for attaching UTXO inputs/outputs to express-invoke-contract RPC endpoint

## [0.8] - 2019-09-13

Initial Release