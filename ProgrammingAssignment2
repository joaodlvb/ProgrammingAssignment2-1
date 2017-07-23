## Caching the Inverse of a Matrix

## Matrix inversion is usually a costly computation and there may be some benefit 
## to caching the inverse of a matrix rather than computing it repeatedly 
## This function creates another matrix to can take its inverse.

makeCacheMatrix <- function(x = matrix()) {
        inv <- NULL
        set <- function (y) {
                x <<- y
                inv <- NULL
                
        }
        get <- function () x
        setInverse <- function(Inverse) inv <<- Inverse
        getInverse <- function () inv
        list (set = set, get = get, setInverse = setInverse, getInverse = getInverse)
}
        
        


## This function compute the inverse of the another matriz created

cacheSolve <- function(x, ...) {
        ## Return a matrix that is the inverse of 'x'
        inv <- x$getInverse()
        if (!is.null(inv)) {
                message ("gettind data")
                return (inv)
        }
        mattriz <- x$get ()
        inv <- solve (mattriz,...)
        x$setInverse(inv)
        inv

}

