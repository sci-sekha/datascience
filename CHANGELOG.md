`datascience` ChangeLog
=======================

All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

## [Unreleased]
None yet.

## v0.7.0
### Changed
- Added predicates for string comparison: `containing` and `contained_in`. (#231)

## v0.6.0
### Changed
- Added `make_array` to make arrays without lists. (#224)
- `Table.select`, `drop`, and `with_columns` now accept variable arguments in addition to lists. (#224)

## v0.5.3
### Changed
- Allow charting methods to select particular columns and default to
  `overlay=True` (#193)
- Make the `values` arg for `pivot` optional. Counting is the default behavior.
  (#191)

### Removed
- The query manager (`Q` class) is removed since no one used it, ever.

## v0.5.1
### Added
- New Table interface: with_columns, labels, column, relabeled

### Changed
- Table.__init__ takes labels as its first argument

### Deprecated
- Two-argument Table.__init__
- Table.empty
- Table.from_rows
- Table.from_columns_dict
- Table.__getattr__
- Table.points
- Table.column_labels renamed to labels
- Table.values renamed to column
- Table.with_relabeling renamed to relabeled

## v0.4.0
### Added
- This CHANGELOG file!
- Docs are now up on [readthedocs][rtd].
- [`util.table_apply` function][table_apply]

[rtd]: http://datascience.readthedocs.org/en/latest/index.html
[table_apply]: https://github.com/data-8/datascience/blob/f7c11b5132299dab0c75a5862cdab9c5b619c7e5/datascience/util.py#L62-L82

