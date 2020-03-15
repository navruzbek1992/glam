

## "Generalized Lehmann's Alternative Model" 

This library estimates asymmetry and location of random variables based on non-parametric approach.
Theoretical development is presented in Miura and Tsukahara (1993). 


## Installation

Steps:

- devtools is required in order to install glam package from github. (library(devtools))
- install_github('navruzbek1992/glam3')
- load the library (library(glam3))


## Example

First generate random numbers and apply glam function. Glam function requries par value to start optimization and type of h function. H function could be chosen as "first", "second" and "third". 

mydata = rnorm(100, 2,3) ## normal dist.

glam_func(mydata, par=c(mean(mydata),1), h_fun = 'first')

Function returns location and asymmetry of random numbers' distribution. Random numberd could be generated from other distirbutions in order to see how the package estimates the assymetry based on non-parametric approach.
