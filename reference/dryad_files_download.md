# Download a specific file

Download a specific file

## Usage

``` r
dryad_files_download(ids, ...)
```

## Arguments

- ids:

  (numeric) one or more file ids, required

- ...:

  Further args passed on to
  [crul::verb-GET](https://docs.ropensci.org/crul/reference/verb-GET.html)

## Value

a list of lists, each named by the input DOI

## Note

UPDATE: we used to not use caching in this fxn; we do now as of
2020-12-15

## See also

Other dryad-files:
[`dryad_files()`](https://docs.ropensci.org/rdryad/reference/dryad_files.md)

## Examples

``` r
if (FALSE) { # \dontrun{
dryad_files_download(ids = 61858)
dryad_files_download(ids = 61859)
} # }
```
