

## Generalized Lehmann's Alternative Model

This library contains tools to estimate asymmetry and location of random variables based on non-parametric approach.
Theoretical development ofthis approach is presented in [Miura and Tsukahara (1993)](http://www3.stat.sinica.edu.tw/statistica/j3n1/j3n17/j3n17.htm). 


## Installation

Steps:

- devtools is required in order to install glam package from github. 
- install the glam package
- load it

```bash
library(devtools)
install_github('navruzbek1992/glam')
library(glam)
```


## Example

First generate random numbers and apply glam function. Glam function requires par value to start optimization and type of h function. H function could be chosen as "first", "second" and "third". 

```bash
data = rnorm(100, 2,3) ## generate random variables from normal distribution.

glam_func(mydata, par=c(mean(data),1), h_fun = 'first')
```
Function returns location and asymmetry of random numbers' distribution. Random numbers could be generated from other distributions in order to check how this library estimates the asymmetry based on non-parametric approach.
