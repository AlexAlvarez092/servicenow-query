# Changelog

## 1.1.1 - 2026-10-21

### Fixed

- `syslog` recipe is now time-bounded and uses `--no-count` (the unbounded query timed out).

## 1.1.0 - 2026-10-21

### Added

- Recipes for `sys_properties`, Flow Designer errors (`sys_flow_context`) and `syslog`.
- Note about custom-domain instance URLs.

### Changed

- Flags verified against `now-sdk` 4.13.6 `query --help`; all recipes tested live.

## 1.0.0 - 2026-10-21

### Added

- Initial release.
