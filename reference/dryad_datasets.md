# List datasets

List datasets

## Usage

``` r
dryad_datasets(...)
```

## Arguments

- ...:

  Named key-value sequeunce of parameters passed to Dryad query such as
  "page" (nunber), or "per_page".

## Value

a tibble

## See also

Other dryad-datasets:
[`dryad_dataset()`](https://docs.ropensci.org/rdryad/reference/dryad_dataset.md),
[`dryad_dataset_versions()`](https://docs.ropensci.org/rdryad/reference/dryad_dataset_versions.md)

## Examples

``` r
if (FALSE) { # \dontrun{
(x <- dryad_datasets())
x$meta
x$links
x$data
x <- dryad_datasets(per_page = 50, page = 7)
} # }
```
