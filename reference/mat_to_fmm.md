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
mat <- matrix(c(1, 2, 3, 4), nrow = 2)
mat_to_fmm(mat, tempfile(fileext = ".mtx"))
#> [1] TRUE
```
