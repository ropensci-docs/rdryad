# Changelog

## rdryad 1.0.0.00x (current dev version)

#### BUG FIXES

- Improve errors on file download
  ([\#43](https://github.com/ropensci/rdryad/issues/43); thanks to
  [@CeresBarros](https://github.com/CeresBarros))

------------------------------------------------------------------------

## rdryad 1.0.0

CRAN release: 2020-06-25

#### BREAKING CHANGES

- Package redone to work with new Dryad API v2. Most functions are
  defunct, and there’s three sets of new functions following the three
  major sets of API routes for datasets, versions, and files. See
  [`?rdryad`](https://docs.ropensci.org/rdryad/reference/rdryad-package.md)
  for more ([\#28](https://github.com/ropensci/rdryad/issues/28))
  ([\#29](https://github.com/ropensci/rdryad/issues/29))

## rdryad 0.4.0

CRAN release: 2018-06-18

#### NEW FEATURES

- gains new function
  [`dryad_metadata()`](https://docs.ropensci.org/rdryad/reference/dryad_metadata-defunct.md)
  to download Dryad file metadata
- gains new function
  [`dryad_package_dois()`](https://docs.ropensci.org/rdryad/reference/dryad_package_dois-defunct.md)
  to get file DOIs for a Dryad package DOI (a package can have many
  files) ([\#22](https://github.com/ropensci/rdryad/issues/22))

#### MINOR IMPROVEMENTS

- `dryad_files` (formerly
  [`download_url()`](https://docs.ropensci.org/rdryad/reference/download_url.md))
  now scrapes Dryad page to get URLs to Dryad files instead of using
  their API, which was not dependable
  ([\#26](https://github.com/ropensci/rdryad/issues/26))
- `dryad_fetch` gains a parameter `try_file_names` (a boolean) which if
  `TRUE` we try to extract file names out of URLs
  ([\#26](https://github.com/ropensci/rdryad/issues/26))

#### BUG FIXES

- fix to solr `rdryad` functions to hard code use of `xml` return
  format, and followlocation to follow any redirects
  ([\#27](https://github.com/ropensci/rdryad/issues/27))

#### DEFUNCT

- [`download_url()`](https://docs.ropensci.org/rdryad/reference/download_url.md)
  is now defunct, see
  [`dryad_files()`](https://docs.ropensci.org/rdryad/reference/dryad_files.md)

#### NOTE

- two new pacakage dependencies: `tibble` and `data.table`

## rdryad 0.3.0

CRAN release: 2017-11-07

#### NEW FEATURES

- Move to using `solrium` package instead of `solr` package for
  interaction with Dryad’s Solr backend
  ([\#21](https://github.com/ropensci/rdryad/issues/21))
  ([\#24](https://github.com/ropensci/rdryad/issues/24))
- Now using `crul` instead of `httr` for HTTP requests
  ([\#23](https://github.com/ropensci/rdryad/issues/23))
- gains two new functions `handle2doi` and `doi2handle` to convert
  between handles and DOIs, and DOIs and handles, respectively
  ([\#25](https://github.com/ropensci/rdryad/issues/25))
- `download_url` function name has been changed to `dryad_files`, but
  you can still use `download_url` until the next version. In addition,
  `download_url`/`dryad_files` parameters `id` is changed to `doi`.

#### MINOR IMPROVEMENTS

- `dryad_fetch` is improved, and uses
  [`curl::curl_download`](https://jeroen.r-universe.dev/curl/reference/curl_download.html)
  instead of `download.file`. It now accepts \>1 input URL, but
  `destile` length must equal number of urls.

## rdryad 0.2.0

CRAN release: 2015-12-23

#### NEW FEATURES

- Re-worked most of the package.
- New package API, some methods are the same, but many are different.
  ([\#16](https://github.com/ropensci/rdryad/issues/16))
- New functions (see functions starting with `d_*()`) to interact with
  Dryad Solr search engine
  ([\#10](https://github.com/ropensci/rdryad/issues/10))
- OAI-PMH functions now using internally the `oai` package.
  ([\#14](https://github.com/ropensci/rdryad/issues/14))

#### MINOR IMPROVEMENTS

- Slimmed down dependencies to a smaller set.
- Changed license from CC0 to MIT
  ([\#17](https://github.com/ropensci/rdryad/issues/17))
- Added more tests
  ([\#18](https://github.com/ropensci/rdryad/issues/18))
- Changed function to get files to only download them, and not attempt
  to read them into R, which introduces a very long dependency chain
  ([\#15](https://github.com/ropensci/rdryad/issues/15))

## rdryad 0.1.1

CRAN release: 2013-01-30

#### BUG FIXES

- removed read.jpeg as a dependency

## rdryad 0.1

CRAN release: 2012-02-23

#### NEW FEATURES

- released to CRAN
