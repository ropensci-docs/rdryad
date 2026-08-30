# Defunct OAI-PMH functions

Defunct OAI-PMH functions

Download metadata for individual Dryad id's

Learn about the Dryad OAI-PMH service.

List Dryad records

Gets OAI Dryad identifiers

Get available Dryad metadata formats

List the sets in the Dryad metadata repository.

## Usage

``` r
dr_get_records(...)

dr_identify(...)

dr_list_records(
  prefix = "oai_dc",
  from = NULL,
  until = NULL,
  set = "hdl_10255_3",
  token = NULL,
  as = "df",
  ...
)

dr_list_identifiers(
  prefix = "oai_dc",
  from = NULL,
  until = NULL,
  set = "hdl_10255_3",
  token = NULL,
  as = "df",
  ...
)

dr_list_metadata_formats(...)

dr_list_sets(token = NULL, as = "df", ...)
```

## Arguments

- ...:

  ignored

## Details

The Dryad OAI-PMH service is no longer being updated See
http://wiki.datadryad.org/Old:Dryad_API#OAI-PMH

Defunct functions:

- `dr_get_records`

- `dr_identify`

- `dr_list_records`

- `dr_list_identifiers`

- `dr_list_metadata_formats`

- `dr_list_sets`
