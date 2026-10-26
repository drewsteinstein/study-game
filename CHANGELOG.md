# Changelog

## v0.1.1 — preserved Dropbox baseline
- Fixed aggregate accuracy normalization so total correct answers cannot exceed total answers.
- Added a regression test for malformed saved counters.
- Reported checks: JavaScript syntax checks passed; Node test suite passed (10 tests, 0 failures); ZIP integrity passed.
- Remaining limitation: real-file browser loading and disk-backed persistence need manual verification in an ordinary browser.
- Source package remains preserved in Dropbox; it has not yet been imported into this repository.
