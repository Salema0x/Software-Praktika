# eVault common utilities

Shared Java utilities used by the [eVault desktop application](../wallet/).

## Components

- Event dispatch and application logging
- File, byte-array, reflection, and serialization helpers
- Encryption and password-based encryption utilities
- ZIP archive support

Source is under [src/main/java/org/mhisoft/common](src/main/java/org/mhisoft/common/); tests are under [src/test/java](src/test/java/).

## Build

The Maven module depends on a parent configuration at `../parent-pom/pom.xml`, which is absent from this repository. Restore the matching upstream parent project before resolving dependencies or running the tests.

## Attribution and license

Originally part of [MHISoft eVault](https://github.com/mhisoft/evault-project). Distributed under the [Apache License 2.0](LICENSE).
