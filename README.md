# Software-Praktika — eVault coursework source snapshot

A historical Java desktop project snapshot retained for software-practicum reference. The included application and utility library originate from **MHISoft eVault**; this repository does not claim original authorship of those upstream components.

## Repository layout

| Directory | Contents |
| --- | --- |
| [wallet](wallet/) | Java Swing password-vault application, UI forms, resources, and TestNG tests |
| [common-utils](common-utils/) | Shared Java utilities and tests |
| [wallet/dist](wallet/dist/) | Historical packaging configuration, launcher script, and screenshots |

## Origin and attribution

- [MHISoft eVault](https://github.com/mhisoft/eVault)
- [MHISoft project referenced by the utility module](https://github.com/mhisoft/evault-project)
- The historical [.gitmodules](.gitmodules) records the original module URLs. The modules in this snapshot are checked-in directories, not active Git submodules.
- Original README files, source headers, and license notices are retained. See [common-utils/LICENSE](common-utils/LICENSE) and the [wallet license section](wallet/README.md#license).

The upstream README includes historical release, donation, and bounty information. Those statements belong to the upstream author and are not new offers by this repository's maintainer.

## Build status and limitations

This is a **legacy source snapshot**, not a verified runnable release. The Maven configuration in `wallet/pom.xml` expects `../parent-pom/pom.xml`, which is absent from this snapshot. Resolve the matching upstream parent configuration and legacy dependencies before attempting a build. No successful build or test run is claimed here.

Historical packaging files refer to bundled Java runtimes and executables that are no longer tracked. They are retained as reference material and require adjustment before packaging. Install a suitable JDK separately.

## Repository cleanup

The November 2026 cleanup:
- moved the project from `OneDrive/Desktop/Repo/evault-project/` to the repository root;
- removed bundled Java runtimes and prebuilt Windows executables from the current tree;
- retained source, tests, assets, build metadata, and upstream attribution;
- added ignore rules for generated output and local development files.

Earlier contents remain recoverable through Git history. This cleanup did not change application logic or establish the security of the historical password-vault implementation.
