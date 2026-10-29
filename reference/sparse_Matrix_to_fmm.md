# Convert a Sparse Numeric Matrix to Matrix Market Format

This function takes a sparse numeric matrix and converts it into a
Matrix Market file.

## Arguments

- input:

  A sparse numeric matrix to be converted.

- filename:

  The name of the output file where the Matrix Market formatted data
  will be saved.

## Value

A boolean indicating success or failure. Writes a MTX file to disk.

## Examples

``` r
sparse_mat <- Matrix::Matrix(c(1, 0, 0, 2), nrow = 2, sparse = TRUE)
sparse_Matrix_to_fmm(sparse_mat, tempfile(fileext = ".mtx"))
#> [1] TRUE
```
