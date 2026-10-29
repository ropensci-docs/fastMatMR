# Convert Matrix Market File to Matrix

This function reads a Matrix Market file and converts it to a matrix in
R.

## Usage

``` r
fmm_to_mat(filename)
```

## Arguments

- filename:

  The name of the input Matrix Market file to be read.

## Value

A matrix containing the data read from the Matrix Market file.

## Examples

``` r
# Create
sample_mat <- matrix(c(1, 2, 3, 4), nrow = 2)
temp_file_mat <- tempfile(fileext = ".mtx")
write_fmm(sample_mat, temp_file_mat)
#> [1] TRUE
# Read
mat <- fmm_to_mat(temp_file_mat)
```
