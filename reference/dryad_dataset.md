# Get datasets by DOI(s)

Get datasets by DOI(s)

## Usage

``` r
dryad_dataset(dois, ...)
```

## Arguments

- dois:

  (character) one or more DOIs, required

- ...:

  Further args passed on to
  [crul::verb-GET](https://docs.ropensci.org/crul/reference/verb-GET.html)

## Value

a list of lists, each named by the input DOI

## See also

Other dryad-datasets:
[`dryad_dataset_versions()`](https://docs.ropensci.org/rdryad/reference/dryad_dataset_versions.md),
[`dryad_datasets()`](https://docs.ropensci.org/rdryad/reference/dryad_datasets.md)

## Examples

``` r
if (FALSE) { # \dontrun{
dryad_dataset(doi = "10.5061/dryad.f385721n")
dois <- c("10.5061/dryad.f385721n", "10.5061/dryad.7ct1n", "10.5061/dryad.1g626")
dryad_dataset(dois = dois)
} # }
```
