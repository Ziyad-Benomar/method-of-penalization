# method-of-penalization
Solving a heat equation where a constraint on a sub-domain is imposed, using variational methods  
(Feb 2020)  
This topic is proposed by François Alouges as a part of the MAP431 course at the Ecole Polytechnique "Variational analysis of partial differential equations".

We are trying to solve the heat equation in a domain Ω by imposing a constraint on a sub-domain B of Ω: the temperature T is set to a value T_B in B.  
The objective of this mini-project is to study a method to perform this resolution using only a Cartesian mesh from Ω. This type of method is very useful in the
case where the B sub-domain is mobile: this avoids having to perform a remeshing to the B sub-domain at every time step.  
We will use freefem++ to make visualize the resulting functions.   


Generally speaking, penalization is a technique for analyzing and solving optimization problems with constraints analytically or numerically. It consists in transforming the problem with constraints into a problem without constraints, where our initial constraint appears in the new function to be optimized in the form of a term multiplied by a constant that we will make tend towards infinity later on.  
In general, we take this constant as the inverse of a positive value epsilon, and we try to show the convergence of the solutions of the penalized problems towards the solution of the initial problem when epsilon tends towards 0.  

