# Convert Matrix Market File to Sparse Matrix

This function reads a Matrix Market file and converts it to a sparse
matrix in R using the Matrix package.

## Usage

``` r
fmm_to_sparse_Matrix(filename)
```

## Arguments

- filename:

  The name of the input Matrix Market file to be read.

## Value

A dgCMatrix object containing the data read from the Matrix Market file.

## Examples

``` r
# Create
sample_sparse_mat <- Matrix::Matrix(c(1, 0, 0, 2), nrow = 2, sparse = TRUE)
temp_file <- tempfile(fileext = ".mtx")
write_fmm(sample_sparse_mat, temp_file)
#> [1] TRUE
# Read
sparse_mat <- fmm_to_sparse_Matrix(temp_file)
```
