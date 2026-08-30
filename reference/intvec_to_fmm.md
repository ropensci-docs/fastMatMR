# Convert a numeric integer vector to Matrix Market Format

This function takes a numeric intvector and converts it into a Matrix
Market output file.

## Arguments

- input:

  A numeric integer vector to be converted.

- filename:

  The name of the output file where the Matrix Market formatted data
  will be saved.

## Value

A boolean indicating success or failure. Writes a MTX file to disk.

## Examples

``` r
intvec <- c(1L, 2L, 3L)
intvec_to_fmm(intvec, tempfile(fileext = ".mtx"))
#> [1] TRUE
```
