# Changelog

## Nov 22th 2017

This push has breaking changes from 0.1.1

Changes:

* Removed types on the response for HttpBuilder.Adapter, to be more flexible
  around errors.
* Removed types on HTTPoison adapter so it doesn't assume response format.

Additions:

* Add HTTPoison adapter.
* Add IBrowse adapter.
* Add Hackney adapter.
* Add JSON Parser adapter, supporting Posion.

* Added with_json_body option.
* Added with_string_body option.
* Added marker to with_body to avoid namespace collision

Deletions:

* removed retry for now, until a proper backoff implementation can be added.
* removed explicit streaming (implicitly still supported), as adapter cannot
  reasonably abstract all possible combinations.
