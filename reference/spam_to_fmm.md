# Convert a spam Sparse Matrix to Matrix Market Format

This function takes a spam sparse matrix and converts it into a Matrix
Market file.

## Usage

``` r
spam_to_fmm(input, filename)
```

## Arguments

- input:

  A spam sparse matrix to be converted.

- filename:

  The name of the output file where the Matrix Market formatted data
  will be saved.

## Value

A boolean indicating success or failure. Writes a MTX file to disk.

## Examples

``` r
sp <- spam::spam(c(1, 0, 0, 2), nrow = 2)
spam_to_fmm(sp, tempfile(fileext = ".mtx"))
#> [1] TRUE
```
