# dryad_download

Download datasets by their DOI(s)

## Usage

``` r
dryad_download(dois, ...)
```

## Arguments

- dois:

  (character) one or more DOIs, required

- ...:

  Further args passed on to
  [crul::verb-GET](https://docs.ropensci.org/crul/reference/verb-GET.html)

## Value

file path for the file

## Examples

``` r
if (FALSE) { # \dontrun{
dryad_download(dois = "10.5061/dryad.f385721n")
dois <- c("10.5061/dryad.f385721n", "10.5061/dryad.7ct1n", "10.5061/dryad.1g626")
dryad_download(dois = dois)
} # }
```
