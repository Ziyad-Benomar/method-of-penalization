# method-of-penalization
Solving a heat equation where a constraint on a sub-domain is imposed, using variational methods  
(Feb 2020)  
This topic is proposed by François Alouges as a part of the MAP431 course at the Ecole Polytechnique "Variational analysis of partial differential equations".

We are trying to solve the heat equation in a domain Ω by imposing a constraint on a sub-domain B of Ω: the temperature T is set to a value T_B in B.  
The objective of this mini-project is to study a method to perform this resolution using only a Cartesian mesh from Ω. This type of method is very useful in the
case where the B sub-domain is mobile: this avoids having to perform a remeshing to the B sub-domain at every time step.  
We will use freefem++ to make visualize the resulting functions.  

