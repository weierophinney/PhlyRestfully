# Changelog

All notable changes to this project will be documented in this file, in reverse chronological order by release.

## 2.3.0 - TBD

### Added

- [#135](https://github.com/phly/PhlyRestfully/pull/135) adds an optional
  `$data = []` parameter to `ResourceController::deleteList()` for consistency
  with other methods.
- [#135](https://github.com/phly/PhlyRestfully/pull/135) adds support for PHP 7
  and HHVM.

### Deprecated

- Nothing.

### Removed

- [#135](https://github.com/phly/PhlyRestfully/pull/135) removes support for PHP
  versions less than 5.5.

### Fixed

- [#135](https://github.com/phly/PhlyRestfully/pull/135) updates all references
  to `Zend\Stdlib\Hydrator` to instead use `Zend\Hydrator`.
- [#135](https://github.com/phly/PhlyRestfully/pull/135) updates all
  `trigger()` and `triggerUntil()` usage with forwards-compatible variants.
- [#97](https://github.com/phly/PhlyRestfully/pull/97) fixes the identifier
  comparison in `ResourceController::getIdentifier()` to use a strict comparison
  to boolean false, and thus allow identifiers of `0`.
- [#104](https://github.com/phly/PhlyRestfully/pull/104) corrects the logic in
  `ResourceParametersListener::detachShared` to pass the identifier.