

## "Generalized Lehmann's Alternative Model" 

This library is a set functions to estimate asymmetry and location of random variables based on non-parametric approach.
Theoretical development is presented in Miura and Tsukahara (1993). 


## Installation

Install devtools first in order to install glam package from github. 

```{r cars}
library(devtools)
install_github('navruzbek1992/glam3')
library(glam3)
```

## Example

Generate random numbers and use glam function. Glam function requries par value to start optimization and type of h function. H function could be chosen as "first", "second" and "third". 

```{r pressure, echo=FALSE}
mydata = rnorm(100, 2,3)
glam_func(mydata, par=c(mean(mydata),1), h_fun = 'first')

```

Function returns location and asymmetry estimates.
