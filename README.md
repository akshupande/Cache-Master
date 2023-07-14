# Cache-Master

This project focuses on creating functions in R that can cache potentially time-consuming computations. It explores the concept of scoping rules in the R language and demonstrates how they can be manipulated to preserve state within an R object.

## Example: Caching the Mean of a Vector

In this, provided two functions, `makeVector` and `cachemean`, to create a special object that stores a numeric vector and caches its mean. The `makeVector` function creates a unique "vector" object, while the `cachemean` function calculates the mean of the vector, utilizing caching to avoid redundant computations.

## Objective: Caching the Inverse of a Matrix

The objective is to write two functions, `makeCacheMatrix` and `cacheSolve`, that cache the inverse of a matrix. The `makeCacheMatrix` function creates a special "matrix" object that can cache its inverse, and the `cacheSolve` function computes the inverse of the matrix, utilizing caching to improve performance.

## Getting Started

To get started with the project, follow these steps:

1. Clone the repository: `git clone https://github.com/akshupande/Cache-Master.git`
2. Navigate to the project directory: `cd Cache-Master`

## Usage

Functions can be used in R code by following these steps:

1. Source the R script containing the functions: `source("caching_functions.R")`
2. Create a special vector object: `v <- makeVector()`
3. Set the value of the vector: `v$set(c(1, 2, 3, 4, 5))`
4. Calculate the mean of the vector, utilizing caching: `cachemean(v)`
5. Retrieve the cached mean: `v$getmean()`

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please submit a pull request.
