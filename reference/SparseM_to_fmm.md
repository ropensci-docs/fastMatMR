# Convert a SparseM matrix.csr to Matrix Market Format

This function takes a SparseM matrix.csr and converts it into a Matrix
Market file.

## Arguments

- input:

  A matrix.csr object to be converted.

- filename:

  The name of the output file where the Matrix Market formatted data
  will be saved.

## Value

A boolean indicating success or failure. Writes a MTX file to disk.

## Examples

``` r
csr <- SparseM::as.matrix.csr(matrix(c(1, 0, 0, 2), nrow = 2))
SparseM_to_fmm(csr, tempfile(fileext = ".mtx"))
#> [1] TRUE
```
