# Get a dataset version by version ID

Get a dataset version by version ID

## Usage

``` r
dryad_versions(ids, ...)

dryad_versions_files(ids, ...)

dryad_versions_download(ids, ...)
```

## Arguments

- ids:

  (numeric/integer) one or more version ids, required

- ...:

  Further args passed on to
  [crul::verb-GET](https://docs.ropensci.org/crul/reference/verb-GET.html)

## Value

a list of lists, each named by the input DOI

## Details

`dryad_versions()` and `dryad_versions_files()` use async http requests,
while `dryad_versions_download()` does not use async

## Examples

``` r
if (FALSE) { # \dontrun{
dryad_versions(ids = 18774)
dryad_versions_files(ids = 18774)
dryad_versions_download(ids = 18774)
} # }
```
