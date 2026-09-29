# Get dataset versions by DOI(s)

Get dataset versions by DOI(s)

## Usage

``` r
dryad_dataset_versions(dois, ...)
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
[`dryad_dataset()`](https://docs.ropensci.org/rdryad/reference/dryad_dataset.md),
[`dryad_datasets()`](https://docs.ropensci.org/rdryad/reference/dryad_datasets.md)

## Examples

``` r
if (FALSE) { # \dontrun{
x = dryad_dataset_versions(dois = "10.5061/dryad.f385721n")
x
dois <- c("10.5061/dryad.f385721n", "10.5061/dryad.7ct1n", "10.5061/dryad.1g626")
dryad_dataset_versions(dois = dois)
} # }
```
