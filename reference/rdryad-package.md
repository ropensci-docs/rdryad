# Interface to the Dryad Web services

Includes access to Dryad's Solr API, OAI-PMH service, and part of their
REST API.

## Package API

The functions match the three major sets of Dryad API routes for
datasets, fiiles and versions.

Datasets:

- [`dryad_dataset()`](https://docs.ropensci.org/rdryad/reference/dryad_dataset.md)

- [`dryad_datasets()`](https://docs.ropensci.org/rdryad/reference/dryad_datasets.md)

- [`dryad_dataset_versions()`](https://docs.ropensci.org/rdryad/reference/dryad_dataset_versions.md)

Files:

- [`dryad_files()`](https://docs.ropensci.org/rdryad/reference/dryad_files.md)

- [`dryad_files_download()`](https://docs.ropensci.org/rdryad/reference/dryad_files_download.md)

Versions:

- [`dryad_versions()`](https://docs.ropensci.org/rdryad/reference/versions.md)

- [`dryad_versions_files()`](https://docs.ropensci.org/rdryad/reference/versions.md)

- [`dryad_versions_download()`](https://docs.ropensci.org/rdryad/reference/versions.md)

## Defunct

The Dryad Solr API is no longer being updated, so the functions that
used to work with it are all defunct, see
[solr-defunct](https://docs.ropensci.org/rdryad/reference/solr-defunct.md)

The Dryad OAI-PMH service is no longer being updated, so the functions
that used to work with it are all defunct, see
[oai-defunct](https://docs.ropensci.org/rdryad/reference/oai-defunct.md)

More defunct functions:

- [`dryad_metadata()`](https://docs.ropensci.org/rdryad/reference/dryad_metadata-defunct.md)

- [`dryad_package_dois()`](https://docs.ropensci.org/rdryad/reference/dryad_package_dois-defunct.md)

- [`handle2doi()`](https://docs.ropensci.org/rdryad/reference/doi2handle-defunct.md)

- [`doi2handle()`](https://docs.ropensci.org/rdryad/reference/doi2handle-defunct.md)

- [`dryad_files()`](https://docs.ropensci.org/rdryad/reference/dryad_files.md)

- [`dryad_fetch()`](https://docs.ropensci.org/rdryad/reference/dryad_fetch-defunct.md) -
  use instead
  [`dryad_files_download()`](https://docs.ropensci.org/rdryad/reference/dryad_files_download.md)
  or
  [`dryad_versions_download()`](https://docs.ropensci.org/rdryad/reference/versions.md)

## See also

Useful links:

- <https://docs.ropensci.org/rdryad>

- <https://github.com/ropensci/rdryad>

- Report bugs at <https://github.com/ropensci/rdryad/issues>

## Author

**Maintainer**: Scott Chamberlain <myrmecocystus@gmail.com>
([ORCID](https://orcid.org/0000-0003-1444-9135))

Authors:

- Scott Chamberlain <myrmecocystus@gmail.com>
  ([ORCID](https://orcid.org/0000-0003-1444-9135))

- Karthik Ram ([ORCID](https://orcid.org/0000-0002-0233-1757))

- Carl Boettiger ([ORCID](https://orcid.org/0000-0002-1642-628X))
