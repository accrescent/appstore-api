<!--
Copyright 2025 Logan Magee

SPDX-License-Identifier: MPL-2.0
-->

# Accrescent Directory API

The Accrescent directory API definitions.

## About

The directory API is the gRPC API used by Accrescent clients to retrieve information about apps
available in the store. Specifically, it allows clients to:

- List apps available for installation in the store
- Retrieve localized app listings for specific apps
- Check for updates
- Fetch app download information
- Determine whether an app is compatible with a device
- ...and more

API definitions are published to [Buf] at the [directory API BSR repository], which also generates
client SDKs.

## Versioning policy

This project uses [Semantic Versioning]. The public API consists of the gRPC API defined in this
repository and the [Buf-generated SDKs] for client implementations but _not_ for server
implementations. That is, API clients will experience breaking changes only in accordance with
Semantic Versioning rules; however, server implementers may experience breaking changes across minor
versions.

[Buf]: https://buf.build
[Buf-generated SDKs]: https://buf.build/accrescent/directory-api/sdks
[directory API BSR repository]: https://buf.build/accrescent/directory-api
[semantic versioning]: https://semver.org
