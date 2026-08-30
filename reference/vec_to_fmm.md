# Convert a Numeric Vector to Matrix Market Format

This function takes a numeric vector and converts it into a Matrix
Market output file.

## Arguments

- input:

  A numeric vector to be converted.

- filename:

  The name of the output file where the Matrix Market formatted data
  will be saved.

## Value

A boolean indicating success or failure. Writes a MTX file to disk.

## Examples

``` r
vec <- c(1, 2, 3)
vec_to_fmm(vec, tempfile(fileext = ".mtx"))
#> [1] TRUE
```
