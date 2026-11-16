# Software-Praktika

Java desktop coursework repository containing a source snapshot of [MHISoft eVault](https://github.com/mhisoft/eVault), an offline password-vault application, and its shared utility library.

## Project overview

The application uses Swing for its desktop interface and includes password-vault management, file attachments, backup/import workflows, and automated tests.

| Component | Contents |
| --- | --- |
| [wallet](wallet/) | Desktop application, UI forms, resources, and tests |
| [common-utils](common-utils/) | Shared utilities for files, events, logging, encryption, and ZIP handling |
| [Packaging assets](wallet/dist/) | Launcher configuration, icons, and application screenshots |

## Technology

Java, Swing, Maven, TestNG, and IntelliJ UI Designer forms.

## Build requirements

Both Maven modules reference `../parent-pom/pom.xml`, which is not included in this snapshot. Restore the matching upstream parent project and resolve the legacy dependencies before building. Packaging scripts also require a separately installed Java runtime and updated local paths.

## Attribution and license

The application and utility library originate from MHISoft eVault. Upstream authorship and source notices are preserved.

- [Original application](https://github.com/mhisoft/eVault)
- [Original project referenced by common-utils](https://github.com/mhisoft/evault-project)
- [Apache 2.0 license](common-utils/LICENSE)
- [Application license notes](wallet/README.md#license)

The entries in [.gitmodules](.gitmodules) document the original module URLs; the modules here are checked-in directories.
