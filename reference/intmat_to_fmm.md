# Convert a Numeric Matrix to Matrix Market Format

This function takes a numeric matrix and converts it into a Matrix
Market file.

## Arguments

- input:

  A numeric matrix to be converted.

- filename:

  The name of the output file where the Matrix Market formatted data
  will be saved.

## Value

A boolean indicating success or failure. Writes a MTX file to disk.

## Examples

``` r
intmat <- matrix(c(1L, 2L, 3L, 4L), nrow = 2)
intmat_to_fmm(intmat, tempfile(fileext = ".mtx"))
#> [1] TRUE
```
