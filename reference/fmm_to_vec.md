# Convert Matrix Market File to Numeric Vector

This function reads a Matrix Market file and converts it to a numeric
vector in R.

## Usage

``` r
fmm_to_vec(filename)
```

## Arguments

- filename:

  The name of the input Matrix Market file to be read.

## Value

A numeric vector containing the data read from the Matrix Market file.

## Examples

``` r
# Create
sample_vec <- c(1, 2, 3)
temp_file_vec <- tempfile(fileext = ".mtx")
write_fmm(sample_vec, temp_file_vec)
#> [1] TRUE
# Read
vec <- fmm_to_vec(temp_file_vec)
```
