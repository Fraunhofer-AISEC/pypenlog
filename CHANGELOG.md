# Changelog

The file uses the format specified in [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## 0.3.2

### Added

* Unit tests with pytest.

### Fixed

* The new RecordType class was not json serializable and `PENLOG_OUTPUT=json` was broken. Fix this problem with `dataclasses.asdict()`.

## 0.3.1

### Fixed

* Use defaults for Optional Types in RecordType to prevent strange errors.

## 0.3.0

### Added

* Linter checks via Github Actions
* This changelog file. :)

### Changed

* The logger now defaults to loglevel INFO. This reflects upcoming changes to the penlog specification.
* Change `penlog.RecordType` to a Python dataclass. Now this type can be imported and extended by other projects.
