# Get metadata information about a file

Get metadata information about a file

## Usage

``` r
dryad_files(ids, ...)
```

## Arguments

- ids:

  (numeric) one or more file ids, required

- ...:

  Further args passed on to
  [crul::verb-GET](https://docs.ropensci.org/crul/reference/verb-GET.html)

## Value

a list of lists, each named by the input DOI

## See also

Other dryad-files:
[`dryad_files_download()`](https://docs.ropensci.org/rdryad/reference/dryad_files_download.md)

## Examples

``` r
if (FALSE) { # \dontrun{
dryad_files(ids = 61859)
dryad_files(ids = 61858)
dryad_files(ids = c(61858, 61859))
} # }
```
