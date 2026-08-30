# Convert Matrix Market File to SparseM matrix.csr

This function reads a Matrix Market file and converts it to a matrix.csr
object using the SparseM package.

## Usage

``` r
fmm_to_SparseM(filename)
```

## Arguments

- filename:

  The name of the input Matrix Market file to be read.

## Value

A matrix.csr object containing the data read from the Matrix Market
file.

## Examples

``` r
sample_sparse <- Matrix::Matrix(c(1, 0, 0, 2), nrow = 2, sparse = TRUE)
tmp <- tempfile(fileext = ".mtx")
write_fmm(sample_sparse, tmp)
#> [1] TRUE
csr <- fmm_to_SparseM(tmp)
```
