# Convert Matrix Market File to spam Sparse Matrix

This function reads a Matrix Market file and converts it to a sparse
matrix using the spam package.

## Usage

``` r
fmm_to_spam(filename)
```

## Arguments

- filename:

  The name of the input Matrix Market file to be read.

## Value

A spam object containing the data read from the Matrix Market file.

## Examples

``` r
sample_sparse <- Matrix::Matrix(c(1, 0, 0, 2), nrow = 2, sparse = TRUE)
tmp <- tempfile(fileext = ".mtx")
write_fmm(sample_sparse, tmp)
#> [1] TRUE
sp <- fmm_to_spam(tmp)
```
