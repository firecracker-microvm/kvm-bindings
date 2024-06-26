# Changelog

## [0.6.0-1]

### Changed

- Specify versionize dependencies via caret requirements instead of
  comparison requirements

## [0.6.0]

### Changed

- [upstream] Updated vmm-sys-utils dependency to 0.11.0
- [upstream] Switched to specifying dependencies using caret requirements
  instead of comparision requirements

### Added

- [upstream] Implement `PartialEq` for fam\_wrappers 

## [0.5.0-1]

- [upstream] updated kvm-bindings to version 0.5.0

## [0.5.0]

### Changed

- Replaced the v4.20 bindings with the v5.13 ones.

### Removed

- Removed v4.14 bindings.

## [0.4.0-1]

- [upstream] vmm-sys-utils dependency bumped to v0.8.0
- versionize dependency bumped to v0.1.6

## [0.4.0]

- vmm-sys-utils dependency bumped to match kvm-ioctls.

## [0.3.0-3]

### Changed

- Upgraded to versionize 0.1.4.
- Implemented Versionize trait for some unions as versionize_derive no longer
  generates union serialization code.

## [0.3.0-2]

### Added

- Added versioning support for kvm bindings structures used
  in VM serialization on arm and arm64.

## [0.3.0-1]

### Added

- [upstream] Enabled `fam-wrappers` support on arm and arm64.
- [upstream] Added fam-wrapper for the arm specific `kvm_reg_list` struct.

## [0.3.0]

### Added

- Added versioning support for kvm bindings structures used
  in VM serialization on x86_64.

## [0.2.0-2]

### Changed

- Updated to `versionize` from crates.io.

## [0.2.0-1]

Built on top of upstream rust-vmm/kvm-bindings v0.2.0.

## [0.2.0]

### Added

- Added opt-in feature `fam-wrappers` that enables exporting
  safe wrappers over generated structs with flexible array
  members. This optional feature has an external dependency
  on `vmm-sys-util`.
- Added safe fam-wrappers for `kvm_msr_list`, `kvm_msrs`,
  and `kvm_cpuid2`.

## [0.1.1]

### Changed

- Do not enforce rust Edition 2018.

## [0.1.0]

### Added

- KVM bindings for Linux kernel version 4.14 and 4.20 with
  support for arm, arm64, x86 and x86_64.
