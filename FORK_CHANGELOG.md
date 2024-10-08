## 1.22.1 (May 1, 2023)

* Add `quote` option to `parameter` blocks in `postgresql_role` resource with default of `true`.

## 1.22.0 (April 28, 2023)

* Fix: use correct values for default ACL object types and `pg_class` kinds.
* Add support for role-scoped configuration parameters.

## 1.21.0 (🔥April 20🔥, 2023)

* Fixed bug causing unexpected revocations when a new grant resource was added
* Merged from [upstream v.1.19.0](https://github.com/cyrilgdn/terraform-provider-postgresql/commit/cb85b9f45ee77b761d8ce08fd74f65350e152256)
* Allow replacing already existing functions on initial resource creation

## 1.20.0 (January 11, 2023)

* Properly support column privileges for views (and materialized views, foreign tables, and partitioned tables)
* Grants for functions now allow function signatures to be provided.
* Merged from [upstream v1.18.0](https://github.com/cyrilgdn/terraform-provider-postgresql/commit/83f06753691b48f7caea7616e6fd443a085761a0)

## 1.19.0 (November 1, 2022)

* Enable update-in-place for changes to grants that only affect `objects`, `columns`, and/or `privileges`.

## 1.18.1 (October 25, 2022)

* Fix identifier quoting in column-level privilege statements

## 1.18.0 (August 30, 2022)

* Add support for column-level privileges
* Forked from 1.17.1, incorporating [column privileges feature](https://github.com/kda-jt/terraform-provider-postgresql/tree/feat-add-column-level-management) by @kda-jt
