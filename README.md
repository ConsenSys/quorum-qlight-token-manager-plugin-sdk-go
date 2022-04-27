# Go SDK for Quorum QLight Token Manager plugins

## Quickstart

```
# qlight-token-manager plugin sdk
go get github.com/ConsenSys/quorum-qlight-token-manager-plugin-sdk-go/proto

# plugin initialization sdk
go get github.com/ConsenSys/quorum-qlight-token-manager-plugin-sdk-go/proto_common

# mocks for testing
go get github.com/ConsenSys/quorum-qlight-token-manager-plugin-sdk-go/mock_proto
```

## Overview

[Quorum's pluggable architecture](https://docs.goquorum.consensys.net/en/latest/Concepts/Plugins/Plugins/) allows for a Quorum node to be extended with additional functionality.

`qlight-token-manager` plugins provide an implementation of management of refresh OAuth Token for QLight clients.

The communication between Quorum and a `qlight-token-manager` plugin uses gRPC.

This SDK can be used to develop Go `qlight-token-manager` plugins that fulfill Quorum's gRPC `qlight-token-manager` plugin interface.  It provides the necessary Go types and methods for starting a new gRPC server, initializing a new plugin, and for handling Quorum gRPC requests.

***This repo is auto-updated***

*The [quorum-plugin-definitions](https://github.com/ConsenSys/quorum-plugin-definitions) project defines the `qlight-token-manager` plugin gRPC API.  A [GitHub Actions workflow](.github/workflows/run.yml) updates the SDK whenever quorum-plugin-definitions is altered.*